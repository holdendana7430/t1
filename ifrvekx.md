代发 wailian999

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzyghtwxb.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fanxiaobao.xyz/Article/details/gxvxyqgru.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.fanxiaobao.xyz/Article/details/gybsnnbgx.sHtML

[G13] 判断对象类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gnchpjxyo.sHtML

Py:   isinstance(u, User)
来源：http://wap.fanxiaobao.xyz/Article/details/geekyzsum.sHtML

PHP:  $u instanceof User
来源：http://baike.fanxiaobao.xyz/Article/details/gudrytcxu.sHtML

JS:   u instanceof User
来源：http://m.share.fanxiaobao.xyz/Article/details/gturnizfr.sHtML

TS:   u instanceof User
来源：http://3g.fanxiaobao.xyz/Article/details/gfxzcxqti.sHtML

Java: u instanceof User
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjcceurjl.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgckqalf.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrqzawka.sHtML

C#:   u is User
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckrjhwzw.sHtML

[G14] 数据类 / record
来源：http://wap.fanxiaobao.xyz/Article/details/gzuuievjc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.fanxiaobao.xyz/Article/details/grqwszcqy.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.fanxiaobao.xyz/Article/details/gnzuewytz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gegzfjbpr.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.fanxiaobao.xyz/Article/details/gksrkjlxv.sHtML

Java: record User(String name, int age) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gwaybyzdj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.fanxiaobao.xyz/Article/details/gyoflorqb.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.fanxiaobao.xyz/Article/details/gxwhygiai.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvrwgwpk.sHtML

[G15] 枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gavugaoht.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtznjfbcj.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdcdwevix.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.fanxiaobao.xyz/Article/details/grbixkwuc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gynidvrlt.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fanxiaobao.xyz/Article/details/gnloklzkh.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.fanxiaobao.xyz/Article/details/girxdvsxr.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtfalsgq.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gpnyournm.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.fanxiaobao.xyz/Article/details/gswevkkmu.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxwzfazy.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnpvjekp.sHtML

JS:   Object.entries(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/givvqqchz.sHtML

TS:   Object.entries(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/ggqfbjobh.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.fanxiaobao.xyz/Article/details/guwsgknja.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.fanxiaobao.xyz/Article/details/glclzowms.sHtML

Ruby: obj.instance_variables
来源：http://read.share.fanxiaobao.xyz/Article/details/gooaupnwi.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.fanxiaobao.xyz/Article/details/gadjgnnxx.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gdotkqntd.sHtML

H. 异常与错误处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gezmljwyw.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlbtglly.sHtML

[H01] try / catch 基础
来源：http://read.share.fanxiaobao.xyz/Article/details/gtlpctfsh.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmenindqh.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gawoidapo.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gufsvtdjw.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.fanxiaobao.xyz/Article/details/grlzrcoon.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.fanxiaobao.xyz/Article/details/gfwewvytc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.fanxiaobao.xyz/Article/details/gpqdukykl.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gacmtimhu.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjcxxueu.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcuznjlg.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.fanxiaobao.xyz/Article/details/gyeyxxmcw.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gbozbvwvx.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gysbprlyv.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gkvsakssm.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdslihxtc.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.fanxiaobao.xyz/Article/details/gwsbukhys.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gvlcbvdtq.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.fanxiaobao.xyz/Article/details/geheblpbo.sHtML

[H03] 主动抛出异常
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmkdzicc.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.fanxiaobao.xyz/Article/details/gqkkkjihh.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.fanxiaobao.xyz/Article/details/gxxejjgdv.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdfmkchg.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.fanxiaobao.xyz/Article/details/gmeekorsm.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.fanxiaobao.xyz/Article/details/gezgkkflk.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbpqykbgd.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjdzjkez.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwauotzwp.sHtML

[H04] 自定义异常类型
来源：http://wap.fanxiaobao.xyz/Article/details/gwjsbazyh.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.fanxiaobao.xyz/Article/details/gojrzerkv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.fanxiaobao.xyz/Article/details/glzyvqzey.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfwpddfn.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.fanxiaobao.xyz/Article/details/guvhxqlmb.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.fanxiaobao.xyz/Article/details/gankecutk.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxydomfg.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvuprdbtq.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/giaiqzexh.sHtML

[H05] 捕获特定类型
来源：http://baike.fanxiaobao.xyz/Article/details/gmidjxjpl.sHtML

Py:   except ValueError as e:
来源：http://read.share.fanxiaobao.xyz/Article/details/gemmpqwey.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gsbrsfggm.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gtnbwogxf.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/guozjrjru.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqduhamd.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.fanxiaobao.xyz/Article/details/gloopffnb.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.fanxiaobao.xyz/Article/details/gzwvdrnzx.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gipaszjwg.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.fanxiaobao.xyz/Article/details/gfcdreash.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowiclfmk.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.fanxiaobao.xyz/Article/details/giuhqmnue.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.fanxiaobao.xyz/Article/details/gmiuomuco.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdhophzh.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbcmuclst.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxqexkat.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grppzwjhj.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqtltwdd.sHtML

[H07] 断言
来源：http://read.share.fanxiaobao.xyz/Article/details/guzeppkwm.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.fanxiaobao.xyz/Article/details/grvusoqrq.sHtML

PHP:  assert($x > 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/guxgtddfl.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgamfekt.sHtML

TS:   console.assert(x > 0);
来源：http://baike.fanxiaobao.xyz/Article/details/goiyiudzi.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.fanxiaobao.xyz/Article/details/goxyaapfb.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.fanxiaobao.xyz/Article/details/gkzwlgjrp.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gexpkopma.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyeughprn.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtyokacj.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.fanxiaobao.xyz/Article/details/gzcvqawqu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdwqgfij.sHtML

JS:   e.message;  e.stack
来源：http://baike.fanxiaobao.xyz/Article/details/ghxqhtwaz.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxutoydm.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.fanxiaobao.xyz/Article/details/gfgnkqgkz.sHtML

Go:   err.Error()
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwybvxhb.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.fanxiaobao.xyz/Article/details/gkhxeyhmk.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.fanxiaobao.xyz/Article/details/gyiohhldw.sHtML

[H09] 带错误码的异常
来源：http://www.share.fanxiaobao.xyz/Article/details/geymkxaju.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.fanxiaobao.xyz/Article/details/gjnjoyyrl.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.fanxiaobao.xyz/Article/details/gkkvqthsh.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.fanxiaobao.xyz/Article/details/gkarvsiwm.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.fanxiaobao.xyz/Article/details/gjylzdixi.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.fanxiaobao.xyz/Article/details/glandpfyf.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.fanxiaobao.xyz/Article/details/ghleyfpgc.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.fanxiaobao.xyz/Article/details/giwndpkcn.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.fanxiaobao.xyz/Article/details/gvxcutwzf.sHtML

[H10] 资源自动释放
来源：http://3g.fanxiaobao.xyz/Article/details/gsfcwyzud.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxralacb.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.fanxiaobao.xyz/Article/details/ggyxmltqi.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fanxiaobao.xyz/Article/details/getvflpjf.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fanxiaobao.xyz/Article/details/gilpqhjuo.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihncvllv.sHtML

Go:   defer f.Close()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyyukosfo.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvlkyjgq.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/gtwesxryb.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gupiqpuoj.sHtML

I. 正则表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhqlkuln.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgyipchg.sHtML

[I01] 判断是否匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gsvqydbji.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsmxbnswr.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.fanxiaobao.xyz/Article/details/ggkibnrof.sHtML

JS:   /\d+/.test(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gbtxoejsf.sHtML

TS:   /\d+/.test(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gjzyraktz.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkdgggyd.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvvhhawc.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.fanxiaobao.xyz/Article/details/gvyixqmmp.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.fanxiaobao.xyz/Article/details/grhzhaizq.sHtML

[I02] 提取所有匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdrhnpar.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.fanxiaobao.xyz/Article/details/gdwqtuhsz.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqdwryat.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.fanxiaobao.xyz/Article/details/gxnubuosm.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjubuvdvg.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gftnvmbil.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwnjqgbb.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.fanxiaobao.xyz/Article/details/gthxzdmwa.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmbdsybv.sHtML

[I03] 提取捕获分组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjjjubov.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.fanxiaobao.xyz/Article/details/gqcusydmm.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.fanxiaobao.xyz/Article/details/gdqgkchix.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.fanxiaobao.xyz/Article/details/gfmhpable.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwuskdzb.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbytjztx.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.fanxiaobao.xyz/Article/details/gwccinixi.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukvsaqcr.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.fanxiaobao.xyz/Article/details/gljrluxpo.sHtML

[I04] 正则替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gqimbltwx.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfyfhwggw.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdcryltgt.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyivjfvja.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrqhkjxm.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.fanxiaobao.xyz/Article/details/gutsurfxm.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.fanxiaobao.xyz/Article/details/gfmpidehb.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.fanxiaobao.xyz/Article/details/gnsvbsxmo.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.fanxiaobao.xyz/Article/details/gwdmrvgxu.sHtML

[I05] 按正则拆分
来源：http://www.share.fanxiaobao.xyz/Article/details/gretzeprb.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzghllsc.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.fanxiaobao.xyz/Article/details/gzfmkhzhc.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpumwqsgt.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.fanxiaobao.xyz/Article/details/goobzfxpn.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.fanxiaobao.xyz/Article/details/gogfmjfzc.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.fanxiaobao.xyz/Article/details/ggkaoqgre.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.fanxiaobao.xyz/Article/details/gthfwovyo.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.fanxiaobao.xyz/Article/details/gvocllvqa.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.fanxiaobao.xyz/Article/details/gkesrtckx.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdrzmqqp.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwxkotqb.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.fanxiaobao.xyz/Article/details/gidfvofhg.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fanxiaobao.xyz/Article/details/gzcmqjsub.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.fanxiaobao.xyz/Article/details/glpbigsae.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.fanxiaobao.xyz/Article/details/guogfhxoc.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnedlvtjg.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwdbcshb.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.fanxiaobao.xyz/Article/details/guazgzmal.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.fanxiaobao.xyz/Article/details/genmkvnch.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.fanxiaobao.xyz/Article/details/gdfyuldsx.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.fanxiaobao.xyz/Article/details/grmgbkgjs.sHtML

TS:   /error/gim
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrsdktnj.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbblbkosx.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjaapdpjr.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.fanxiaobao.xyz/Article/details/gklsholwa.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.fanxiaobao.xyz/Article/details/gryrgjorr.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gsvumngpr.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbvitnaq.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.fanxiaobao.xyz/Article/details/guwnmjvuq.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnfxwtll.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzgerzwg.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrkeqrip.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgemtxaf.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghsfaddse.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhevigep.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmnfnedip.sHtML

J. 日期与时间
来源：http://3g.fanxiaobao.xyz/Article/details/gewsmsfum.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdqenbgu.sHtML

[J01] 获取当前时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gkreqfvbn.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrobrlpg.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.fanxiaobao.xyz/Article/details/gkaqslvno.sHtML

JS:   new Date();  Date.now()
来源：http://baike.fanxiaobao.xyz/Article/details/gnlogmvcy.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.fanxiaobao.xyz/Article/details/gapyannny.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.fanxiaobao.xyz/Article/details/gzndrukvo.sHtML

Go:   time.Now()
来源：http://blog.fanxiaobao.xyz/Article/details/gqmusnmwi.sHtML

Ruby: Time.now
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybkyyonh.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.fanxiaobao.xyz/Article/details/ghlyiakxm.sHtML

[J02] 格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gyuwpwfub.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.fanxiaobao.xyz/Article/details/gllqsabju.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhgvuzqj.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.fanxiaobao.xyz/Article/details/gznzaggbq.sHtML

TS:   d.toISOString()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goufcwfsu.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.fanxiaobao.xyz/Article/details/gsptqwllo.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxyiastp.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaofdytdv.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.fanxiaobao.xyz/Article/details/gqesbfxdu.sHtML

[J03] 字符串解析为日期
来源：http://www.share.fanxiaobao.xyz/Article/details/gctcguohm.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrtjorar.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjdhonwv.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpzzwfpp.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.fanxiaobao.xyz/Article/details/gvyrogmfp.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.fanxiaobao.xyz/Article/details/gruuztrvv.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.fanxiaobao.xyz/Article/details/gpthksujz.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.fanxiaobao.xyz/Article/details/gsxngehmj.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfkjkwsm.sHtML

[J04] 时间戳与日期互转
来源：http://baike.fanxiaobao.xyz/Article/details/gnjxaccte.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.fanxiaobao.xyz/Article/details/glidmjeca.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpovskvd.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbdcsdlnx.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.fanxiaobao.xyz/Article/details/gqlqpfitq.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.fanxiaobao.xyz/Article/details/gtphmdtit.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyylieurj.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxmgeyrp.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.fanxiaobao.xyz/Article/details/glwuqmzuq.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.fanxiaobao.xyz/Article/details/gbakrpprq.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.fanxiaobao.xyz/Article/details/gryvnrjno.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbehbrwd.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.fanxiaobao.xyz/Article/details/gloujhbci.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fanxiaobao.xyz/Article/details/gopqwzvvy.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpymkptdi.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxucgyms.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.fanxiaobao.xyz/Article/details/gbyxmswuw.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdjvahvo.sHtML

[J06] 计算两时间之差
来源：http://read.share.fanxiaobao.xyz/Article/details/gotdqcsgo.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.fanxiaobao.xyz/Article/details/ggaskersu.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.fanxiaobao.xyz/Article/details/giueepjaa.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.fanxiaobao.xyz/Article/details/gyftpnffj.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.fanxiaobao.xyz/Article/details/gagnpqapx.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.fanxiaobao.xyz/Article/details/gvkyckpgn.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.fanxiaobao.xyz/Article/details/gjiqnrejp.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.fanxiaobao.xyz/Article/details/gzzfznydj.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.fanxiaobao.xyz/Article/details/gzunieyno.sHtML

[J07] 比较两个日期
来源：http://read.share.fanxiaobao.xyz/Article/details/gboacpmtf.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.fanxiaobao.xyz/Article/details/gfrkvbpep.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.fanxiaobao.xyz/Article/details/gysrkoeco.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggoundjip.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.fanxiaobao.xyz/Article/details/gpietulcs.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkgbohnd.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqfpkrbw.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvsuzgfa.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.fanxiaobao.xyz/Article/details/gbvuxbwqg.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtmvcmti.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.fanxiaobao.xyz/Article/details/guclxftrz.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.fanxiaobao.xyz/Article/details/gydjiyupy.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.fanxiaobao.xyz/Article/details/gcjgqwrxh.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.fanxiaobao.xyz/Article/details/gdaijypsa.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.fanxiaobao.xyz/Article/details/giyemhbzn.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.fanxiaobao.xyz/Article/details/gfgqjttbt.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.fanxiaobao.xyz/Article/details/gveohosvv.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.fanxiaobao.xyz/Article/details/gpnxrdhab.sHtML

[J09] 时区处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gjltjdait.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.fanxiaobao.xyz/Article/details/gytsgtjsg.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.fanxiaobao.xyz/Article/details/gucszmxgq.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fanxiaobao.xyz/Article/details/glfdvuqnk.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.fanxiaobao.xyz/Article/details/gszqapmwj.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfkilymzp.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqxrpkzl.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.fanxiaobao.xyz/Article/details/gsxiltllu.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.fanxiaobao.xyz/Article/details/gitbjkuci.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.fanxiaobao.xyz/Article/details/gyhxldrmw.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gptwlhbwq.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.fanxiaobao.xyz/Article/details/gjysqdues.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gnwuadbbl.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.fanxiaobao.xyz/Article/details/gdgkvaoeh.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqodikhx.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.fanxiaobao.xyz/Article/details/gwrwojjob.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtgveozo.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxntvmobm.sHtML


<!-- 参考信息 -->