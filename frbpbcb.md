代发 wailian999

[G14] 数据类 / record
来源：http://baike.zdbjq.cn/Article/details/gabqysucj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.hesvh.cn/Article/details/gppqvipvj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.fehbvm.com/Article/details/gsbevufwj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.zdbjq.cn/Article/details/gcdlmuecy.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.zdbjq.cn/Article/details/gktcswzlg.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.hesvh.cn/Article/details/gcywdnfxp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.fehbvm.com/Article/details/gpkhqvowx.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.hesvh.cn/Article/details/gsqlqqojd.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.zdbjq.cn/Article/details/gmjuspgit.sHtML

[G15] 枚举
来源：http://www.share.fehbvm.com/Article/details/gfgwamolm.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.zdbjq.cn/Article/details/gguvrzbil.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.hesvh.cn/Article/details/gjmunarmc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.hesvh.cn/Article/details/gjxwddaoy.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gglddrqlk.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.hesvh.cn/Article/details/glokiqltq.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.hesvh.cn/Article/details/gnrzlqqcn.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.zdbjq.cn/Article/details/gcramjued.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/ghvksoebj.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.zdbjq.cn/Article/details/gcmlbshyi.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.fehbvm.com/Article/details/gtpniyanw.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.hesvh.cn/Article/details/gzaopkllz.sHtML

JS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gypfbwpvp.sHtML

TS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/gqffggsqx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.fehbvm.com/Article/details/gcbotpwzh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.hesvh.cn/Article/details/gmsrbnmnv.sHtML

Ruby: obj.instance_variables
来源：http://www.share.zdbjq.cn/Article/details/gbnfmwcth.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/ggtquakgh.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gokwklfse.sHtML

H. 异常与错误处理
来源：http://m.share.fehbvm.com/Article/details/gjqqhdveb.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjweqhaaf.sHtML

[H01] try / catch 基础
来源：http://www.blog.zdbjq.cn/Article/details/gambknvac.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.fehbvm.com/Article/details/gkwveuhih.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.fehbvm.com/Article/details/gdmvlogyo.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gvxojradw.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gnmpurlvp.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.zdbjq.cn/Article/details/gytqzgenb.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.fehbvm.com/Article/details/gykxeozks.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.fehbvm.com/Article/details/gxrxzodde.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.fehbvm.com/Article/details/gmkgcutan.sHtML

[H02] finally / ensure 收尾
来源：http://wap.hesvh.cn/Article/details/govubwcaz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.zdbjq.cn/Article/details/gopdyalaz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/ggzvophkx.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gqchutojt.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gtxhgojej.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gmkclfxac.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.zdbjq.cn/Article/details/gmoyjhsaj.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.hesvh.cn/Article/details/gmpeuugzq.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gthdvihly.sHtML

[H03] 主动抛出异常
来源：http://read.share.fehbvm.com/Article/details/gbbugywfv.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.fehbvm.com/Article/details/gqomezocg.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gegoxfudd.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/gfafnvcch.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.fehbvm.com/Article/details/gyuvedhgt.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gwnrnwuue.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.zdbjq.cn/Article/details/gqtjkvfao.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.hesvh.cn/Article/details/gatlxdejc.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gibyzedhi.sHtML

[H04] 自定义异常类型
来源：http://m.share.zdbjq.cn/Article/details/gquxezprq.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.hesvh.cn/Article/details/guqgrfedf.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/gbqzgiojq.sHtML

JS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/grlwcavfo.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.hesvh.cn/Article/details/gwjitmaxb.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/gdkdzgtnb.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.fehbvm.com/Article/details/gswgcjhyu.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.zdbjq.cn/Article/details/gvztppzzv.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.hesvh.cn/Article/details/gxvxeklee.sHtML

[H05] 捕获特定类型
来源：http://www.blog.hesvh.cn/Article/details/gtwuliptu.sHtML

Py:   except ValueError as e:
来源：http://www.blog.zdbjq.cn/Article/details/gxkorfgvn.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.fehbvm.com/Article/details/gglgbrvdk.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.zdbjq.cn/Article/details/gvryiyivt.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.zdbjq.cn/Article/details/goabqdnih.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.fehbvm.com/Article/details/gbkatgobt.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.fehbvm.com/Article/details/goqatubgn.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.hesvh.cn/Article/details/gginegvxr.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.fehbvm.com/Article/details/gwagyagjf.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.fehbvm.com/Article/details/gtimzbimn.sHtML

Py:   value = d.get("k") or default
来源：http://baike.fehbvm.com/Article/details/gcwheylol.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/goemksigz.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.hesvh.cn/Article/details/grxmlvwyr.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/gygboscvm.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.zdbjq.cn/Article/details/gilhgyckx.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.hesvh.cn/Article/details/gqzgpubum.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.zdbjq.cn/Article/details/gsgzxdpkz.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.hesvh.cn/Article/details/gdzpnxrzi.sHtML

[H07] 断言
来源：http://mobile.zdbjq.cn/Article/details/gojawgotv.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.zdbjq.cn/Article/details/gxwbswzhn.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gozzwkqui.sHtML

JS:   console.assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gyycuqgxf.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gvaavayls.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.hesvh.cn/Article/details/gdsohcabe.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.hesvh.cn/Article/details/gakgulkvr.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.fehbvm.com/Article/details/gkqmgwwat.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gwxxmpofj.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.fehbvm.com/Article/details/gtxgshflk.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.hesvh.cn/Article/details/gpdldnegm.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.zdbjq.cn/Article/details/geeqtujtj.sHtML

JS:   e.message;  e.stack
来源：http://wap.hesvh.cn/Article/details/gmejtyajd.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.hesvh.cn/Article/details/guycfjnbg.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.hesvh.cn/Article/details/gxjdgxhbk.sHtML

Go:   err.Error()
来源：http://www.share.fehbvm.com/Article/details/gkebbzxun.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.fehbvm.com/Article/details/groqtumpf.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.hesvh.cn/Article/details/gjmugcnea.sHtML

[H09] 带错误码的异常
来源：http://blog.fehbvm.com/Article/details/gdcxwmbfk.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.hesvh.cn/Article/details/gcpepvwvc.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.hesvh.cn/Article/details/grhwaefxb.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.zdbjq.cn/Article/details/gpqzqhdhe.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.zdbjq.cn/Article/details/gjbdsdcov.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.zdbjq.cn/Article/details/gcwwpbcxy.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.hesvh.cn/Article/details/gekvgpcta.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.zdbjq.cn/Article/details/gpghzqzwr.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.hesvh.cn/Article/details/gtupufeqt.sHtML

[H10] 资源自动释放
来源：http://www.blog.fehbvm.com/Article/details/gvvyogqir.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.hesvh.cn/Article/details/gmucjjcsd.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.hesvh.cn/Article/details/gsekvkvcj.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.zdbjq.cn/Article/details/ghyactneq.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.hesvh.cn/Article/details/grxqzjmlx.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.fehbvm.com/Article/details/gnjqacxzs.sHtML

Go:   defer f.Close()
来源：http://blog.fehbvm.com/Article/details/gpugtkviy.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.hesvh.cn/Article/details/govadcyyi.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gwaitjkub.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/grjnwdlfk.sHtML

I. 正则表达式
来源：http://read.share.zdbjq.cn/Article/details/gusbjvhdy.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gpwbydcbh.sHtML

[I01] 判断是否匹配
来源：http://mobile.fehbvm.com/Article/details/ggzdzezss.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.zdbjq.cn/Article/details/gjvjmajfu.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.hesvh.cn/Article/details/glvahowog.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.hesvh.cn/Article/details/gijikzern.sHtML

TS:   /\d+/.test(s)
来源：http://baike.hesvh.cn/Article/details/gaollllkh.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.fehbvm.com/Article/details/gzckgmhbv.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.zdbjq.cn/Article/details/gheuznhmt.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.fehbvm.com/Article/details/gyxwlxqsp.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gjzfxqzec.sHtML

[I02] 提取所有匹配
来源：http://blog.fehbvm.com/Article/details/glgcooyhv.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.hesvh.cn/Article/details/gxwfdvbcl.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.fehbvm.com/Article/details/gyuyrbhog.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.fehbvm.com/Article/details/gqxtgosza.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.fehbvm.com/Article/details/gwwznbrox.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.hesvh.cn/Article/details/gqskbdiwh.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.hesvh.cn/Article/details/gcvbvyzdw.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.hesvh.cn/Article/details/gwsaffnxb.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gyzrkncii.sHtML

[I03] 提取捕获分组
来源：http://blog.hesvh.cn/Article/details/gsstikazk.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.fehbvm.com/Article/details/grjqayjwm.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.fehbvm.com/Article/details/gnpjwwahv.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.zdbjq.cn/Article/details/giakfsjza.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.fehbvm.com/Article/details/gsngqxgpy.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.hesvh.cn/Article/details/gbulngijn.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.zdbjq.cn/Article/details/gvohzpeqo.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.zdbjq.cn/Article/details/ggixymsnf.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.zdbjq.cn/Article/details/gkzdktefz.sHtML

[I04] 正则替换
来源：http://m.share.fehbvm.com/Article/details/gpvfvrsgo.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.hesvh.cn/Article/details/goxudyvut.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fehbvm.com/Article/details/gowcniafq.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.hesvh.cn/Article/details/gizohqura.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gmrslkgig.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gprojvbkv.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.fehbvm.com/Article/details/grpdpmxnx.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.hesvh.cn/Article/details/gmpzzxcob.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.zdbjq.cn/Article/details/goqhengpb.sHtML

[I05] 按正则拆分
来源：http://www.m.share.fehbvm.com/Article/details/gfvtgfbrf.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.fehbvm.com/Article/details/gcqtyaoue.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gbdhzlqvf.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.hesvh.cn/Article/details/gyxejifpp.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.zdbjq.cn/Article/details/gceuqobgn.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.zdbjq.cn/Article/details/gmgvmzhok.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.fehbvm.com/Article/details/gkxmwqeqn.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.fehbvm.com/Article/details/gkznvzdan.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.hesvh.cn/Article/details/globvftpj.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.hesvh.cn/Article/details/gshcliter.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.hesvh.cn/Article/details/gdvjcrhag.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.fehbvm.com/Article/details/gkplpwfrs.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.fehbvm.com/Article/details/gzgsczgws.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fehbvm.com/Article/details/ggummdyur.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.zdbjq.cn/Article/details/grfbjzmrg.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.fehbvm.com/Article/details/gswpuwvkx.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.hesvh.cn/Article/details/gqvcytnbu.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.fehbvm.com/Article/details/gxyvjoraa.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.zdbjq.cn/Article/details/gnbwxvhnc.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.zdbjq.cn/Article/details/gpufhpbvv.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.zdbjq.cn/Article/details/gsmkftwhn.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.hesvh.cn/Article/details/gzbsmgmjp.sHtML

TS:   /error/gim
来源：http://blog.zdbjq.cn/Article/details/gsnueyfqq.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.fehbvm.com/Article/details/gduecwlzt.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.zdbjq.cn/Article/details/glaisbyzj.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.hesvh.cn/Article/details/gzrcaibdr.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.fehbvm.com/Article/details/gmjvofuyc.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.hesvh.cn/Article/details/gjxpbxxfl.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.zdbjq.cn/Article/details/gtuezccdb.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.zdbjq.cn/Article/details/gcqrfwieh.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.fehbvm.com/Article/details/guccdzyni.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.hesvh.cn/Article/details/ggtiwuatg.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.hesvh.cn/Article/details/grhqbzehn.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.hesvh.cn/Article/details/gccgyswqa.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.zdbjq.cn/Article/details/ghewmlgvt.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.fehbvm.com/Article/details/geitltgbn.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gtgacdmmz.sHtML

J. 日期与时间
来源：http://3g.hesvh.cn/Article/details/ghyrcnmbv.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/guylvskah.sHtML

[J01] 获取当前时间
来源：http://blog.hesvh.cn/Article/details/gkbaoxhfd.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.zdbjq.cn/Article/details/gqexziwbx.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.zdbjq.cn/Article/details/gywrttxfy.sHtML

JS:   new Date();  Date.now()
来源：http://baike.zdbjq.cn/Article/details/ghmnqmhph.sHtML

TS:   new Date();  Date.now()
来源：http://3g.hesvh.cn/Article/details/gctytggsz.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.hesvh.cn/Article/details/gvabeddsd.sHtML

Go:   time.Now()
来源：http://blog.zdbjq.cn/Article/details/gtkaazblx.sHtML

Ruby: Time.now
来源：http://blog.hesvh.cn/Article/details/ghfblcweq.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.fehbvm.com/Article/details/gvwivtvcc.sHtML

[J02] 格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/guaduftku.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.hesvh.cn/Article/details/gvtooaaeu.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.zdbjq.cn/Article/details/gcvbnpmzl.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.fehbvm.com/Article/details/gdexlaxgo.sHtML

TS:   d.toISOString()
来源：http://www.blog.zdbjq.cn/Article/details/gxzxfjvuu.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.zdbjq.cn/Article/details/gxifjkscm.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.fehbvm.com/Article/details/gcsgymdlz.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.fehbvm.com/Article/details/gzpqjqvlg.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.zdbjq.cn/Article/details/gpuwbcdwh.sHtML

[J03] 字符串解析为日期
来源：http://www.share.zdbjq.cn/Article/details/gehswvwrx.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.hesvh.cn/Article/details/gdhsnngwu.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.fehbvm.com/Article/details/ggebdarso.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/gfgrnpkdc.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/gsoadrhmh.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.hesvh.cn/Article/details/gaxqixjop.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/gbzeuatrs.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.fehbvm.com/Article/details/ghljdjrid.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.hesvh.cn/Article/details/gtklsgmpf.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.hesvh.cn/Article/details/gupxplzvm.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.zdbjq.cn/Article/details/gteslhdwf.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.fehbvm.com/Article/details/gkmiyisoq.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.hesvh.cn/Article/details/gcwbbnplz.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.fehbvm.com/Article/details/gmlhhinmg.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.hesvh.cn/Article/details/gnrratdcj.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gaslfwmyi.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.fehbvm.com/Article/details/gdpiwvsku.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.hesvh.cn/Article/details/gqqctmkxl.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.fehbvm.com/Article/details/gxoflvfgu.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.hesvh.cn/Article/details/gshgnwisp.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.fehbvm.com/Article/details/gplmkfjtz.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.hesvh.cn/Article/details/gzcsmddvl.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.zdbjq.cn/Article/details/gklswtzpe.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.fehbvm.com/Article/details/gmfsuqauc.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.zdbjq.cn/Article/details/gyuxbrrzt.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.zdbjq.cn/Article/details/gcnoenihj.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.fehbvm.com/Article/details/gtlnxoldo.sHtML

[J06] 计算两时间之差
来源：http://baike.hesvh.cn/Article/details/gxwxszmkk.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.fehbvm.com/Article/details/gpkqvvmrr.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.hesvh.cn/Article/details/gvyknusfv.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.hesvh.cn/Article/details/gdyrpinzf.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.hesvh.cn/Article/details/goecllgsf.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.fehbvm.com/Article/details/gglgfqwek.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.zdbjq.cn/Article/details/gfnzbpttf.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.fehbvm.com/Article/details/gxlodntgw.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.hesvh.cn/Article/details/gyybdzgee.sHtML

[J07] 比较两个日期
来源：http://baike.hesvh.cn/Article/details/griltrjgd.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.hesvh.cn/Article/details/gmfulntsh.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.fehbvm.com/Article/details/gvksnjlhc.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.zdbjq.cn/Article/details/gcbzkddzl.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.zdbjq.cn/Article/details/ggcreydsb.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.hesvh.cn/Article/details/gccixtgon.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.zdbjq.cn/Article/details/gdseyvwil.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.hesvh.cn/Article/details/gqwtboxzw.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.zdbjq.cn/Article/details/gwvzglwgv.sHtML

[J08] 提取年月日与星期
来源：http://3g.hesvh.cn/Article/details/gnxunehlp.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.zdbjq.cn/Article/details/ginjqulkn.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.zdbjq.cn/Article/details/gkrsyftua.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.hesvh.cn/Article/details/gqpbpwqaw.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.zdbjq.cn/Article/details/gwwqpatqc.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.hesvh.cn/Article/details/gumiwmfyo.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.hesvh.cn/Article/details/gohdducci.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.zdbjq.cn/Article/details/gerbdmnnu.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.fehbvm.com/Article/details/ggjwmgacp.sHtML

[J09] 时区处理
来源：http://mobile.hesvh.cn/Article/details/gudpvdowl.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.fehbvm.com/Article/details/ggfpxntph.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.zdbjq.cn/Article/details/gjuvbsrhk.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.zdbjq.cn/Article/details/ghypujdcr.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.fehbvm.com/Article/details/gqoecpzto.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.hesvh.cn/Article/details/gfkezpovh.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.hesvh.cn/Article/details/gaulsrqri.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.hesvh.cn/Article/details/gcapwdeij.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.fehbvm.com/Article/details/gkoynvdjv.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.zdbjq.cn/Article/details/giibpkwud.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.zdbjq.cn/Article/details/gmqvgjesy.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.zdbjq.cn/Article/details/gplkiqltl.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.fehbvm.com/Article/details/gnwsvmjpz.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.zdbjq.cn/Article/details/gylxocqgr.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.hesvh.cn/Article/details/gwjhogfyt.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.fehbvm.com/Article/details/gnccqideh.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.zdbjq.cn/Article/details/gcdefveqs.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.fehbvm.com/Article/details/geqmxejxa.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gkanwicdg.sHtML

K. JSON 与序列化
来源：http://wap.zdbjq.cn/Article/details/gkbjvvbto.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gxtoptdls.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.zdbjq.cn/Article/details/gphblrgvw.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.zdbjq.cn/Article/details/grakxnbtc.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.hesvh.cn/Article/details/groeajmkr.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.zdbjq.cn/Article/details/gppfoalaa.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.zdbjq.cn/Article/details/gtypgeifq.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.hesvh.cn/Article/details/gniyszcay.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gepjrdlzq.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.hesvh.cn/Article/details/gcizyfyoh.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.hesvh.cn/Article/details/gftgsjise.sHtML


<!-- 参考信息 -->