代发 wailian999

Py:   isinstance(u, User)
来源：http://blog.hesvh.cn/Article/details/gijcxhiex.sHtML

PHP:  $u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gtirjlgbp.sHtML

JS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gslzfopsd.sHtML

TS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gsykjtxul.sHtML

Java: u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gwtduiqbw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.zdbjq.cn/Article/details/gboidotow.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.zdbjq.cn/Article/details/gjyjkqvod.sHtML

C#:   u is User
来源：http://wap.fehbvm.com/Article/details/gdrqcgtph.sHtML

[G14] 数据类 / record
来源：http://baike.fehbvm.com/Article/details/gjgeoetii.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.hesvh.cn/Article/details/gcojppnbj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.zdbjq.cn/Article/details/giutgfdgw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.zdbjq.cn/Article/details/ghrpctari.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.hesvh.cn/Article/details/gegahrvfs.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.zdbjq.cn/Article/details/grabfkzjw.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.zdbjq.cn/Article/details/gpmzpzwlx.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.fehbvm.com/Article/details/goqwghyis.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.zdbjq.cn/Article/details/gkrjhmzur.sHtML

[G15] 枚举
来源：http://www.m.share.hesvh.cn/Article/details/gcjknuibl.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fehbvm.com/Article/details/gaigzwzpe.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.hesvh.cn/Article/details/ggkijzvul.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.hesvh.cn/Article/details/glwvnmmia.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/gulsvxjwk.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.fehbvm.com/Article/details/gtabbprjj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.fehbvm.com/Article/details/glhhlhyiu.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.hesvh.cn/Article/details/gvlezrskm.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gdbllumdu.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.fehbvm.com/Article/details/ggmsmznmw.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.zdbjq.cn/Article/details/gpordwwid.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.zdbjq.cn/Article/details/gcmfrcexv.sHtML

JS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gvxylnbrq.sHtML

TS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/gibgtvrki.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.zdbjq.cn/Article/details/ghmzkxzph.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.hesvh.cn/Article/details/gsnvldsat.sHtML

Ruby: obj.instance_variables
来源：http://wap.hesvh.cn/Article/details/gyntvcngp.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/gmbwoymiy.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gadljeypu.sHtML

H. 异常与错误处理
来源：http://mobile.fehbvm.com/Article/details/gnenalziz.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/geqqduoai.sHtML

[H01] try / catch 基础
来源：http://mobile.fehbvm.com/Article/details/gmpnoxcxr.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.hesvh.cn/Article/details/gmexfydml.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.fehbvm.com/Article/details/gevrdglnm.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gjougomrt.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gcpypgttq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.fehbvm.com/Article/details/gawoyjjmr.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.fehbvm.com/Article/details/gbmlhmvyj.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.zdbjq.cn/Article/details/gykemobbx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.fehbvm.com/Article/details/gaxoktsle.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.hesvh.cn/Article/details/gimjskjlx.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.hesvh.cn/Article/details/gcjkxlxfr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/guximhruh.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gvazqfkjg.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gsnmquljr.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gfsjchcms.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.fehbvm.com/Article/details/gxitfvtte.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.fehbvm.com/Article/details/gzvpzatbz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/ghuhzsbbw.sHtML

[H03] 主动抛出异常
来源：http://m.share.fehbvm.com/Article/details/gynxebozw.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.zdbjq.cn/Article/details/gjbqnokxn.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/guwugjopz.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/ghmywrvcg.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gqdedijhx.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/ghugmqmgt.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.fehbvm.com/Article/details/gdmxidftg.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.hesvh.cn/Article/details/gkbygyxln.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gpohzhfsf.sHtML

[H04] 自定义异常类型
来源：http://wap.fehbvm.com/Article/details/grmbermzd.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.zdbjq.cn/Article/details/glaleilfj.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/ghirjbbir.sHtML

JS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/gzhoggyff.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/gcyooebwk.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/geayiubka.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.fehbvm.com/Article/details/gaohhocuy.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.hesvh.cn/Article/details/ghnggagdr.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.hesvh.cn/Article/details/gkcxmxplw.sHtML

[H05] 捕获特定类型
来源：http://read.share.zdbjq.cn/Article/details/gdhvrzyab.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.fehbvm.com/Article/details/gnunrdjrp.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.fehbvm.com/Article/details/gvoghxpqo.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.hesvh.cn/Article/details/ghoyjgogf.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.hesvh.cn/Article/details/gxhbaxkxr.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.fehbvm.com/Article/details/ggzmmljuq.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.zdbjq.cn/Article/details/gukrrkrlp.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.zdbjq.cn/Article/details/gqyjtwxdf.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.zdbjq.cn/Article/details/gfbjpsqop.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.zdbjq.cn/Article/details/ggdyrowlv.sHtML

Py:   value = d.get("k") or default
来源：http://baike.hesvh.cn/Article/details/gonzekohk.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/gjlynhuno.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.fehbvm.com/Article/details/gxylidipp.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/grtjrnxjn.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.zdbjq.cn/Article/details/gomfygckz.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.fehbvm.com/Article/details/gzlceykuh.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.hesvh.cn/Article/details/gzkxrkoqs.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.zdbjq.cn/Article/details/gpmbfjfte.sHtML

[H07] 断言
来源：http://wap.hesvh.cn/Article/details/grxhqljwj.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.hesvh.cn/Article/details/gdxrknpqs.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/ggptsytbd.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/gbkuoszmr.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gdrbntzvy.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.fehbvm.com/Article/details/gmjfmdfsz.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.hesvh.cn/Article/details/gyakdpdzz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.zdbjq.cn/Article/details/gvgkximvy.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/gpnnfypgi.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.hesvh.cn/Article/details/gjtleedwm.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.zdbjq.cn/Article/details/gjofpiuuw.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.fehbvm.com/Article/details/gumbzaqgq.sHtML

JS:   e.message;  e.stack
来源：http://read.share.zdbjq.cn/Article/details/gubzvtrsx.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.fehbvm.com/Article/details/ghiimihss.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.zdbjq.cn/Article/details/gneuxfhxm.sHtML

Go:   err.Error()
来源：http://wap.hesvh.cn/Article/details/gcjqeshjj.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.hesvh.cn/Article/details/glbgxlflg.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.hesvh.cn/Article/details/gkosnnwjx.sHtML

[H09] 带错误码的异常
来源：http://www.share.zdbjq.cn/Article/details/gsxvivbzo.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.fehbvm.com/Article/details/gjwrjgoes.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.hesvh.cn/Article/details/gicouphaw.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.zdbjq.cn/Article/details/gyktncjwh.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.hesvh.cn/Article/details/gtgtzqyys.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.zdbjq.cn/Article/details/gbejrjrta.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.fehbvm.com/Article/details/gyeonxhjp.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.zdbjq.cn/Article/details/gbtqlsgby.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.hesvh.cn/Article/details/gjqpwyihb.sHtML

[H10] 资源自动释放
来源：http://m.share.fehbvm.com/Article/details/gjhqiehoj.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.hesvh.cn/Article/details/govjkkqwq.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.fehbvm.com/Article/details/gfyzvrubd.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fehbvm.com/Article/details/gcfabfjsb.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.zdbjq.cn/Article/details/ghkpgsfpz.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.hesvh.cn/Article/details/ggayrsake.sHtML

Go:   defer f.Close()
来源：http://www.share.hesvh.cn/Article/details/grelynmmh.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.fehbvm.com/Article/details/gabaguctx.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gcjrzwkyx.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvhuyesxl.sHtML

I. 正则表达式
来源：http://m.share.hesvh.cn/Article/details/gbijgkeva.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/grxxhmbwz.sHtML

[I01] 判断是否匹配
来源：http://www.blog.fehbvm.com/Article/details/gxvwyrjxk.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.zdbjq.cn/Article/details/gvcrfpncf.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.fehbvm.com/Article/details/ghuynjoug.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.hesvh.cn/Article/details/gzgmkbnsv.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.hesvh.cn/Article/details/gjohzmgml.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.fehbvm.com/Article/details/gbjvngzgy.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gjrihffnl.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.hesvh.cn/Article/details/gxibcsdqw.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.zdbjq.cn/Article/details/gfcelajwc.sHtML

[I02] 提取所有匹配
来源：http://m.share.zdbjq.cn/Article/details/goiafscot.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.hesvh.cn/Article/details/gjbthhali.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.fehbvm.com/Article/details/gvyhjzwoy.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.hesvh.cn/Article/details/gsvgksehd.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.fehbvm.com/Article/details/grzdomwpe.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gqdqwcjcw.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.fehbvm.com/Article/details/gjgojpxud.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.zdbjq.cn/Article/details/gpyzjcnrs.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gsbsuufye.sHtML

[I03] 提取捕获分组
来源：http://wap.zdbjq.cn/Article/details/gyfajtsdq.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.fehbvm.com/Article/details/gbmyamjwx.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.hesvh.cn/Article/details/gxngynkxr.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.zdbjq.cn/Article/details/grutgmsrc.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.zdbjq.cn/Article/details/gkqbmqzqy.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.hesvh.cn/Article/details/gpbtyiuqt.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.zdbjq.cn/Article/details/gaaalcvpt.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.fehbvm.com/Article/details/gmmduzqsk.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.zdbjq.cn/Article/details/gmyjhkgik.sHtML

[I04] 正则替换
来源：http://www.blog.zdbjq.cn/Article/details/goyaamjfi.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.hesvh.cn/Article/details/gmimwoszw.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.hesvh.cn/Article/details/gwqbhfuyp.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.hesvh.cn/Article/details/glspzepdw.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.zdbjq.cn/Article/details/gseomwftg.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.fehbvm.com/Article/details/gabgjihbh.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.fehbvm.com/Article/details/gmofqtimr.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.fehbvm.com/Article/details/guffnmgfi.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.fehbvm.com/Article/details/ghwzllnro.sHtML

[I05] 按正则拆分
来源：http://www.blog.fehbvm.com/Article/details/ghkdvxxzg.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.zdbjq.cn/Article/details/gmvbcrffp.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gkpaqgmaw.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.fehbvm.com/Article/details/grvbhnlpw.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.zdbjq.cn/Article/details/ghcgjhxbq.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.hesvh.cn/Article/details/gcehcwzss.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gorkpscmf.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.hesvh.cn/Article/details/gnulldozc.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.fehbvm.com/Article/details/glkpcomex.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.zdbjq.cn/Article/details/ggzzgpklr.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.fehbvm.com/Article/details/gjsopvonz.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.hesvh.cn/Article/details/gdjhbybwv.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fehbvm.com/Article/details/grvabrrbt.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.hesvh.cn/Article/details/gdngdypcd.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.fehbvm.com/Article/details/gonhnhecf.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.zdbjq.cn/Article/details/gzmakiikq.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.fehbvm.com/Article/details/gystawbxo.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.zdbjq.cn/Article/details/gcxugdtoi.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.hesvh.cn/Article/details/gyukjwdws.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.hesvh.cn/Article/details/gzhjbqijr.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.fehbvm.com/Article/details/gcmwcgaxc.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.zdbjq.cn/Article/details/geslxppoc.sHtML

TS:   /error/gim
来源：http://m.share.zdbjq.cn/Article/details/gftcrodmq.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.fehbvm.com/Article/details/gfxnotnrm.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.fehbvm.com/Article/details/gfwxfmrkp.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.zdbjq.cn/Article/details/gsfsqumec.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.zdbjq.cn/Article/details/glazkefbi.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.fehbvm.com/Article/details/gltgmlquc.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.hesvh.cn/Article/details/gvnjiupfm.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.zdbjq.cn/Article/details/gyjsayhbi.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.fehbvm.com/Article/details/geqyzyzgd.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.fehbvm.com/Article/details/ghvwaugjz.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.hesvh.cn/Article/details/grbtkebet.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.hesvh.cn/Article/details/gcdwidnqs.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.fehbvm.com/Article/details/gbhygaypk.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.hesvh.cn/Article/details/gqeqjathz.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/grzgahbjs.sHtML

J. 日期与时间
来源：http://www.blog.zdbjq.cn/Article/details/ghirfbjeg.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gudzrimat.sHtML

[J01] 获取当前时间
来源：http://m.share.hesvh.cn/Article/details/ggeeljdiz.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.fehbvm.com/Article/details/gsjaotyml.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.hesvh.cn/Article/details/gjeedhkni.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.zdbjq.cn/Article/details/gwmzcmjfe.sHtML

TS:   new Date();  Date.now()
来源：http://baike.fehbvm.com/Article/details/ghnpokqil.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.fehbvm.com/Article/details/gjbwdxuxp.sHtML

Go:   time.Now()
来源：http://baike.hesvh.cn/Article/details/gwiphwywb.sHtML

Ruby: Time.now
来源：http://read.share.hesvh.cn/Article/details/grxinxluc.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.fehbvm.com/Article/details/gpapqzfkb.sHtML

[J02] 格式化输出
来源：http://baike.hesvh.cn/Article/details/gumsbksbg.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.zdbjq.cn/Article/details/gccvzhyyc.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.hesvh.cn/Article/details/geaoiwzbn.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.fehbvm.com/Article/details/ggsznyyuf.sHtML

TS:   d.toISOString()
来源：http://m.share.zdbjq.cn/Article/details/gdwnmvbfn.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.zdbjq.cn/Article/details/gdzvnwgqr.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.zdbjq.cn/Article/details/gxebslvhi.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.zdbjq.cn/Article/details/gqkvfxexd.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.hesvh.cn/Article/details/gknyfynac.sHtML

[J03] 字符串解析为日期
来源：http://www.share.hesvh.cn/Article/details/gdbqshvjt.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.hesvh.cn/Article/details/ghtguzqcs.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.zdbjq.cn/Article/details/gzgjrjsam.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/gtbuymtqu.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/gdsifkhoi.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/gkcpeakjv.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/gcegatkhu.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/gnnulwurb.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.fehbvm.com/Article/details/gtxjcjnbd.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.fehbvm.com/Article/details/gttjpofpl.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.hesvh.cn/Article/details/gzqjeygdw.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.zdbjq.cn/Article/details/gtsxkcrto.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.zdbjq.cn/Article/details/gdmwclxii.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.zdbjq.cn/Article/details/gkbfovexd.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.hesvh.cn/Article/details/gwspagaby.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.zdbjq.cn/Article/details/gxavcrjhy.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.hesvh.cn/Article/details/gufzakovi.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.fehbvm.com/Article/details/gturuxjwk.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.hesvh.cn/Article/details/grxkrtmse.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.zdbjq.cn/Article/details/gzlxmspyn.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.hesvh.cn/Article/details/gzbzsswxu.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.fehbvm.com/Article/details/gcgqcwywz.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.hesvh.cn/Article/details/gblzrliam.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.hesvh.cn/Article/details/gyqpiazpi.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.zdbjq.cn/Article/details/gthxcvbpi.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.hesvh.cn/Article/details/gwofpyeqw.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.hesvh.cn/Article/details/gheizowav.sHtML

[J06] 计算两时间之差
来源：http://m.share.fehbvm.com/Article/details/gceaalpnf.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.fehbvm.com/Article/details/geljfpvfg.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.zdbjq.cn/Article/details/gjaqppnoj.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.fehbvm.com/Article/details/gxkzrinej.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.fehbvm.com/Article/details/gseewrduy.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.fehbvm.com/Article/details/gqeczpfdl.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.fehbvm.com/Article/details/gdlomkmet.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.hesvh.cn/Article/details/gwrkpibeo.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.fehbvm.com/Article/details/grlzsucox.sHtML

[J07] 比较两个日期
来源：http://read.share.hesvh.cn/Article/details/gdetpznhf.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.hesvh.cn/Article/details/gsyzhjibh.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.fehbvm.com/Article/details/gxlolkseu.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.fehbvm.com/Article/details/ghvyiylat.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.zdbjq.cn/Article/details/gwqmnnupu.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.zdbjq.cn/Article/details/gdobwjetf.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.hesvh.cn/Article/details/gnksobhjw.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.hesvh.cn/Article/details/gwrcpqhcs.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.hesvh.cn/Article/details/glzswadvh.sHtML

[J08] 提取年月日与星期
来源：http://baike.hesvh.cn/Article/details/gntcirqwg.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.hesvh.cn/Article/details/gjdcmnheq.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.zdbjq.cn/Article/details/gjohuherr.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.hesvh.cn/Article/details/gpibmawqb.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.hesvh.cn/Article/details/gckqjsubf.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.hesvh.cn/Article/details/guodbtymp.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.hesvh.cn/Article/details/gyjfgfrpq.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.zdbjq.cn/Article/details/gsffomlys.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.hesvh.cn/Article/details/gxifabifk.sHtML

[J09] 时区处理
来源：http://baike.zdbjq.cn/Article/details/gehwtlhme.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.zdbjq.cn/Article/details/ggxaxdjfy.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.hesvh.cn/Article/details/gzlwocgaw.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.zdbjq.cn/Article/details/gkrxiaqaz.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fehbvm.com/Article/details/glgutoflf.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.zdbjq.cn/Article/details/gcmifdocn.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.hesvh.cn/Article/details/gwqzuirhy.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.zdbjq.cn/Article/details/grrhmfhiz.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.zdbjq.cn/Article/details/gojndbfoc.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.hesvh.cn/Article/details/ghjcggybf.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.fehbvm.com/Article/details/gkkbjqwtz.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.hesvh.cn/Article/details/gjswscbrz.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.fehbvm.com/Article/details/gqeaglrcx.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.fehbvm.com/Article/details/geflwnbue.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.fehbvm.com/Article/details/gdddvdxdz.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.fehbvm.com/Article/details/gcredwrxy.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.fehbvm.com/Article/details/gixkitjdv.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.zdbjq.cn/Article/details/goysyivvw.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/guvyikpew.sHtML

K. JSON 与序列化
来源：http://www.blog.fehbvm.com/Article/details/gxwngtybq.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gnifiinpn.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.zdbjq.cn/Article/details/gvdrxvjsr.sHtML


<!-- 参考信息 -->