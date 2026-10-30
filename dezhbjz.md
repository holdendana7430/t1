代发 wailian999

[G14] 数据类 / record
来源：http://3g.fanxiaobao.xyz/Article/details/gcccxzrln.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.fanxiaobao.xyz/Article/details/giwceipyf.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.fanxiaobao.xyz/Article/details/gnxjejhbp.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.fanxiaobao.xyz/Article/details/gzpumhixj.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.fanxiaobao.xyz/Article/details/gedpjrydi.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gggutrqws.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrbsondh.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.fanxiaobao.xyz/Article/details/gztgynkwc.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnlfnful.sHtML

[G15] 枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwozxvic.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwiwbwvl.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnirbrcuf.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.fanxiaobao.xyz/Article/details/gytqwrgip.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbtsxkws.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.fanxiaobao.xyz/Article/details/gmlbmlxig.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvokqlpyn.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfahvseev.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gwovdjjjv.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.fanxiaobao.xyz/Article/details/gtxsmnhai.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.fanxiaobao.xyz/Article/details/gckmgkluc.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.fanxiaobao.xyz/Article/details/gecrgfnah.sHtML

JS:   Object.entries(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gaqghhfnj.sHtML

TS:   Object.entries(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gjzohgdyo.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.fanxiaobao.xyz/Article/details/gncoiufac.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.fanxiaobao.xyz/Article/details/ghovrynbk.sHtML

Ruby: obj.instance_variables
来源：http://blog.fanxiaobao.xyz/Article/details/giogjizkj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.fanxiaobao.xyz/Article/details/gwpbizksp.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gviocqgrh.sHtML

H. 异常与错误处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdsijbjbq.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/ggcjqqagj.sHtML

[H01] try / catch 基础
来源：http://baike.fanxiaobao.xyz/Article/details/goaozbgxn.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvhmryod.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyavtrbis.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.fanxiaobao.xyz/Article/details/gqaocrpop.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzadrgily.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjnswhof.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.fanxiaobao.xyz/Article/details/gcqtxyhnr.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.fanxiaobao.xyz/Article/details/gusvroegm.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.fanxiaobao.xyz/Article/details/gwhwxdhcq.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gpnswmzvs.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.fanxiaobao.xyz/Article/details/gkncqowue.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gexviqjdu.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gczbrgxcq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginvytjdq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfthfpxfs.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.fanxiaobao.xyz/Article/details/gsphxsqxm.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gcolpcnnz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrwtqhar.sHtML

[H03] 主动抛出异常
来源：http://3g.fanxiaobao.xyz/Article/details/gvwgmbhug.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.fanxiaobao.xyz/Article/details/gxuzdgzvk.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.fanxiaobao.xyz/Article/details/gshahnltq.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.fanxiaobao.xyz/Article/details/ggdovbsic.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxcugvyn.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.fanxiaobao.xyz/Article/details/gtzqiqdix.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.fanxiaobao.xyz/Article/details/gixqijrim.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.fanxiaobao.xyz/Article/details/guikkqnqz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.fanxiaobao.xyz/Article/details/grvuykpwy.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbubuslvs.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.fanxiaobao.xyz/Article/details/gesmvusgn.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgighqip.sHtML

JS:   class MyError extends Error {}
来源：http://3g.fanxiaobao.xyz/Article/details/ggmptryvb.sHtML

TS:   class MyError extends Error {}
来源：http://3g.fanxiaobao.xyz/Article/details/gesbolqjg.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.fanxiaobao.xyz/Article/details/guquqhdva.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.fanxiaobao.xyz/Article/details/gexmsqalm.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfoyczbn.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gjthwaoiq.sHtML

[H05] 捕获特定类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gtrrzcgon.sHtML

Py:   except ValueError as e:
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfgkkuce.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.fanxiaobao.xyz/Article/details/gyogsuzoy.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/geuvjnrlw.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gqicyrijc.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvpweusf.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfukpaig.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggsslwxrz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwyulcqd.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.fanxiaobao.xyz/Article/details/gaanwshyn.sHtML

Py:   value = d.get("k") or default
来源：http://blog.fanxiaobao.xyz/Article/details/gyqyzaqki.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.fanxiaobao.xyz/Article/details/gktednwrs.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpjppsju.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.fanxiaobao.xyz/Article/details/gxyiksjyk.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.fanxiaobao.xyz/Article/details/glbhnurfp.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwduewyrs.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.fanxiaobao.xyz/Article/details/gkixeiegn.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzizgpbgq.sHtML

[H07] 断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrothcss.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.fanxiaobao.xyz/Article/details/gplaxgmid.sHtML

PHP:  assert($x > 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpxgnssv.sHtML

JS:   console.assert(x > 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gjsucrgrw.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbqdbchs.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.fanxiaobao.xyz/Article/details/gniskujmg.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.fanxiaobao.xyz/Article/details/govnbzndb.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmxiahwx.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdtbydtx.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.fanxiaobao.xyz/Article/details/gowhhorsx.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.fanxiaobao.xyz/Article/details/gqbimbzls.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdsqmlvvw.sHtML

JS:   e.message;  e.stack
来源：http://mobile.fanxiaobao.xyz/Article/details/gyeexukub.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.fanxiaobao.xyz/Article/details/gktttmxls.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.fanxiaobao.xyz/Article/details/gdkjvwfwf.sHtML

Go:   err.Error()
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxcdzihy.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.fanxiaobao.xyz/Article/details/gsjebxzqf.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbmixpppy.sHtML

[H09] 带错误码的异常
来源：http://read.share.fanxiaobao.xyz/Article/details/guyyeervd.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.fanxiaobao.xyz/Article/details/gqeonvzfj.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.fanxiaobao.xyz/Article/details/gdtzjkftd.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqmcwmiu.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gesaqwpxe.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.fanxiaobao.xyz/Article/details/grmxzkjwb.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gkiycweas.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnkdbuno.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.fanxiaobao.xyz/Article/details/gmempoexj.sHtML

[H10] 资源自动释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjycdlte.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.fanxiaobao.xyz/Article/details/glexvddwq.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.fanxiaobao.xyz/Article/details/gntnpqegl.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fanxiaobao.xyz/Article/details/gbslnyzcm.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fanxiaobao.xyz/Article/details/gjpcdnhgt.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtiazjcyt.sHtML

Go:   defer f.Close()
来源：http://blog.fanxiaobao.xyz/Article/details/guoffmpxl.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.fanxiaobao.xyz/Article/details/gomklouvb.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnaxtutfi.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/glvjgajrm.sHtML

I. 正则表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gvrtqjmlm.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gkksevfdz.sHtML

[I01] 判断是否匹配
来源：http://wap.fanxiaobao.xyz/Article/details/glvncwpvi.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvvaldql.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.fanxiaobao.xyz/Article/details/gcrwbursw.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gulaeuzyz.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdabsvjae.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.fanxiaobao.xyz/Article/details/ghthskysh.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gcaircyfw.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzczdrmg.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gevyrqino.sHtML

[I02] 提取所有匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gewaghsok.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.fanxiaobao.xyz/Article/details/ggyhpckvt.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.fanxiaobao.xyz/Article/details/goiimnejp.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcldgqxhy.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxjsqvnv.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjpvcmet.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.fanxiaobao.xyz/Article/details/ginkvznan.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzsttllx.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwggteua.sHtML

[I03] 提取捕获分组
来源：http://www.share.fanxiaobao.xyz/Article/details/golzkdpdn.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.fanxiaobao.xyz/Article/details/gtvasrfdl.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgafipjm.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.fanxiaobao.xyz/Article/details/gzwhmwrvf.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagmynuzr.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.fanxiaobao.xyz/Article/details/gnkezttmo.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvszkyvn.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.fanxiaobao.xyz/Article/details/grkdizhni.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtapyuli.sHtML

[I04] 正则替换
来源：http://mobile.fanxiaobao.xyz/Article/details/ggpmgxipy.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gidcqstku.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gghilbmpt.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.fanxiaobao.xyz/Article/details/glmykalkq.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbqsoraq.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.fanxiaobao.xyz/Article/details/gkxmmcroc.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.fanxiaobao.xyz/Article/details/gfxrsiojf.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbqzoykc.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjrztqwv.sHtML

[I05] 按正则拆分
来源：http://www.share.fanxiaobao.xyz/Article/details/gajetbmzn.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gonebkwyx.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.fanxiaobao.xyz/Article/details/grlpabjem.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.fanxiaobao.xyz/Article/details/goftpppcd.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvhzpykp.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.fanxiaobao.xyz/Article/details/guffzowvy.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijogeoju.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.fanxiaobao.xyz/Article/details/gzuzduxzl.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.fanxiaobao.xyz/Article/details/gtyyjmyer.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.fanxiaobao.xyz/Article/details/gllwskiga.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.fanxiaobao.xyz/Article/details/gurbxrbxs.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.fanxiaobao.xyz/Article/details/ggfmmxvig.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fanxiaobao.xyz/Article/details/gwysxglbd.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkiwlikzz.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqaxydfcy.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.fanxiaobao.xyz/Article/details/guiyuocpv.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.fanxiaobao.xyz/Article/details/gxehrvxki.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbidneepa.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.fanxiaobao.xyz/Article/details/gtzknuehb.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnehmjmv.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcracfxlp.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcxdouzv.sHtML

TS:   /error/gim
来源：http://blog.fanxiaobao.xyz/Article/details/gcnybxzsb.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdlqycav.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxsxngfq.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsskvstyl.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.fanxiaobao.xyz/Article/details/gaxdklorn.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gttlniqfj.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.fanxiaobao.xyz/Article/details/giluzqqcy.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwsmjpot.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.fanxiaobao.xyz/Article/details/gwszzzunt.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtdmlmgb.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.fanxiaobao.xyz/Article/details/gyggzukub.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.fanxiaobao.xyz/Article/details/gmdinioxs.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvuvcocbh.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.fanxiaobao.xyz/Article/details/gghzuawir.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjhntvko.sHtML

J. 日期与时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibjibdgv.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gmyknbuyf.sHtML

[J01] 获取当前时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gooixbdeq.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.fanxiaobao.xyz/Article/details/grttxlgwc.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.fanxiaobao.xyz/Article/details/gblcbqtxv.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.fanxiaobao.xyz/Article/details/gptorostb.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxkiziwbu.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.fanxiaobao.xyz/Article/details/gvpxjjtvs.sHtML

Go:   time.Now()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwurkpxig.sHtML

Ruby: Time.now
来源：http://baike.fanxiaobao.xyz/Article/details/gyehkeqys.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.fanxiaobao.xyz/Article/details/gzejaffaa.sHtML

[J02] 格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gloxlwpfl.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupohsokz.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.fanxiaobao.xyz/Article/details/gwvwgmbeo.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvsppnzr.sHtML

TS:   d.toISOString()
来源：http://wap.fanxiaobao.xyz/Article/details/getvvwdfi.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.fanxiaobao.xyz/Article/details/glozqtzex.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.fanxiaobao.xyz/Article/details/gadrakpfe.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.fanxiaobao.xyz/Article/details/gbiysjsfw.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbupavqm.sHtML

[J03] 字符串解析为日期
来源：http://blog.fanxiaobao.xyz/Article/details/gewwqaxmb.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.fanxiaobao.xyz/Article/details/geiwholaf.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.fanxiaobao.xyz/Article/details/gxwqjxlky.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.fanxiaobao.xyz/Article/details/gafwtytln.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpibeeoc.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfbzraea.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnkgkovw.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhjprpir.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.fanxiaobao.xyz/Article/details/gjucftiok.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctlzavyh.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grapvzxbi.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.fanxiaobao.xyz/Article/details/glodmossl.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbduroowr.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.fanxiaobao.xyz/Article/details/girsgpmyc.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbrbjvgrh.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvhulbdq.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.fanxiaobao.xyz/Article/details/gzsciaenr.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbzysydxj.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.fanxiaobao.xyz/Article/details/gqggtghjz.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.fanxiaobao.xyz/Article/details/gltbbdcwj.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkymxszx.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdujxvcao.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gspxvlfia.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.fanxiaobao.xyz/Article/details/gaswsbhtv.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.fanxiaobao.xyz/Article/details/garhviwdx.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.fanxiaobao.xyz/Article/details/gerdlteau.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzgkcnsq.sHtML

[J06] 计算两时间之差
来源：http://baike.fanxiaobao.xyz/Article/details/gvokxsryv.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsozwavha.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgwjlfdd.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvcvmnxra.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywscexqh.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.fanxiaobao.xyz/Article/details/grvgjezhg.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.fanxiaobao.xyz/Article/details/gfrakhmpe.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdhmsqwa.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfcjptikk.sHtML

[J07] 比较两个日期
来源：http://www.blog.fanxiaobao.xyz/Article/details/guoxdaben.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbblosmld.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.fanxiaobao.xyz/Article/details/gransixtu.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.fanxiaobao.xyz/Article/details/grnkzcsdx.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.fanxiaobao.xyz/Article/details/gmekcybui.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdepwoawf.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.fanxiaobao.xyz/Article/details/gsrpvvncj.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbcayypq.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfojbzvfa.sHtML

[J08] 提取年月日与星期
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdhbqdyf.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.fanxiaobao.xyz/Article/details/ggqxrrcjn.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppuylszk.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjefxqfyl.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.fanxiaobao.xyz/Article/details/gkncbjpzn.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.fanxiaobao.xyz/Article/details/gbyevhrma.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbwmrkfa.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.fanxiaobao.xyz/Article/details/grbiluwlb.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.fanxiaobao.xyz/Article/details/gcuimyyoo.sHtML

[J09] 时区处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcuhqkfsp.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.fanxiaobao.xyz/Article/details/gsuknpmzm.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgaxdrbt.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.fanxiaobao.xyz/Article/details/grnrmppcb.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvnzwxjz.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvmvxeuw.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.fanxiaobao.xyz/Article/details/gddbjhvmi.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkdclqep.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.fanxiaobao.xyz/Article/details/gkrgnolzx.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.fanxiaobao.xyz/Article/details/gvjwuxtxq.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpnhikff.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.fanxiaobao.xyz/Article/details/garnnxhsc.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/geptxdkkm.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.fanxiaobao.xyz/Article/details/gdsnvhacn.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtbarllq.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.fanxiaobao.xyz/Article/details/gbuinfbzg.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.fanxiaobao.xyz/Article/details/gvcvyejav.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gllupkfap.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gkilrpgnn.sHtML

K. JSON 与序列化
来源：http://wap.fanxiaobao.xyz/Article/details/ggudltspc.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmznwxnnr.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gcziedqot.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.fanxiaobao.xyz/Article/details/gxkcvglnm.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.fanxiaobao.xyz/Article/details/golhmtasa.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxshoyecs.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gmrsyhios.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.fanxiaobao.xyz/Article/details/gixscyuph.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdxgzdeji.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnywecacy.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/guwzkknuc.sHtML


<!-- 参考信息 -->