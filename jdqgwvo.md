代发 wailian999

Py:   isinstance(u, User)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmyoaaad.sHtML

PHP:  $u instanceof User
来源：http://blog.fanxiaobao.xyz/Article/details/gnthgmxmo.sHtML

JS:   u instanceof User
来源：http://3g.fanxiaobao.xyz/Article/details/gxcznlilu.sHtML

TS:   u instanceof User
来源：http://mobile.fanxiaobao.xyz/Article/details/gctwqaspy.sHtML

Java: u instanceof User
来源：http://m.share.fanxiaobao.xyz/Article/details/geztkstop.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.fanxiaobao.xyz/Article/details/gxyegmsqo.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxhvtgzi.sHtML

C#:   u is User
来源：http://m.share.fanxiaobao.xyz/Article/details/gvfvxknfw.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwkrukan.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.fanxiaobao.xyz/Article/details/goqddycmk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtrcwudo.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fanxiaobao.xyz/Article/details/gxtlfnsic.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.fanxiaobao.xyz/Article/details/gokwsvnuq.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvziaiwu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.fanxiaobao.xyz/Article/details/gmpiwtuix.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gromatdyw.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.fanxiaobao.xyz/Article/details/gjmgfewir.sHtML

[G15] 枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gxgmaoqhh.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqmatoxr.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzokxysd.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtedwjsy.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gtdqtlefe.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljsrzful.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpyfvtet.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.fanxiaobao.xyz/Article/details/gqdipycms.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmctlyzqm.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfiomxhr.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fanxiaobao.xyz/Article/details/gbwwzrenl.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.fanxiaobao.xyz/Article/details/gimgyxjjs.sHtML

JS:   Object.entries(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gvrktlycn.sHtML

TS:   Object.entries(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/glonnorqb.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvyjhsad.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghycicbzh.sHtML

Ruby: obj.instance_variables
来源：http://wap.fanxiaobao.xyz/Article/details/gyhvvqtng.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.fanxiaobao.xyz/Article/details/gfwxsdxhx.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gfmvtewoh.sHtML

H. 异常与错误处理
来源：http://blog.fanxiaobao.xyz/Article/details/gupxfiyrf.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgyqrzwz.sHtML

[H01] try / catch 基础
来源：http://m.share.fanxiaobao.xyz/Article/details/gbgaknzax.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkjfidtu.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gpfsvgibk.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.fanxiaobao.xyz/Article/details/gmzgtdcia.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojkpxlbi.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdegbyrm.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.fanxiaobao.xyz/Article/details/gueegzxmb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkngpsog.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.fanxiaobao.xyz/Article/details/gipvvgtqi.sHtML

[H02] finally / ensure 收尾
来源：http://3g.fanxiaobao.xyz/Article/details/gyfvkaydw.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.fanxiaobao.xyz/Article/details/gvskebbpj.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gtvtzqzrd.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndzzkqfp.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gbcawvexo.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.fanxiaobao.xyz/Article/details/glzkxfhqd.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmktxzac.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.fanxiaobao.xyz/Article/details/gciwynpgv.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gzgemddzn.sHtML

[H03] 主动抛出异常
来源：http://3g.fanxiaobao.xyz/Article/details/ghpnzyhoe.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.fanxiaobao.xyz/Article/details/glrfmtzyb.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.fanxiaobao.xyz/Article/details/gmiyvreno.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.fanxiaobao.xyz/Article/details/glktcwshu.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.fanxiaobao.xyz/Article/details/gqcrynqax.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdsciyri.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.fanxiaobao.xyz/Article/details/guacxcjha.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxleylim.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.fanxiaobao.xyz/Article/details/gevttqnfo.sHtML

[H04] 自定义异常类型
来源：http://baike.fanxiaobao.xyz/Article/details/gxzxjkgku.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.fanxiaobao.xyz/Article/details/gzisvhvgb.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.fanxiaobao.xyz/Article/details/gilizapsw.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gurxojtka.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gboumnozp.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfsvxyoew.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.fanxiaobao.xyz/Article/details/glfsjqzga.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.fanxiaobao.xyz/Article/details/gboswxvvz.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gglzecryn.sHtML

[H05] 捕获特定类型
来源：http://wap.fanxiaobao.xyz/Article/details/gmkpmxtwq.sHtML

Py:   except ValueError as e:
来源：http://baike.fanxiaobao.xyz/Article/details/gnphmegjz.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwzgssft.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gpacnqune.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.fanxiaobao.xyz/Article/details/geebhfwci.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzmdlyju.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzebuzhly.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowdvjwvn.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gycuivjnh.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.fanxiaobao.xyz/Article/details/gpndtchsv.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxxnweqh.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.fanxiaobao.xyz/Article/details/gmtqycprn.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrezmldb.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspylcinm.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.fanxiaobao.xyz/Article/details/gdweqvzei.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdihowbvw.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnwdzftqq.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.fanxiaobao.xyz/Article/details/gifrdjwpf.sHtML

[H07] 断言
来源：http://read.share.fanxiaobao.xyz/Article/details/gigwoqafz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.fanxiaobao.xyz/Article/details/gsouttoht.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkisefdun.sHtML

JS:   console.assert(x > 0);
来源：http://wap.fanxiaobao.xyz/Article/details/gbmvhrhlr.sHtML

TS:   console.assert(x > 0);
来源：http://wap.fanxiaobao.xyz/Article/details/gjfuixpid.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.fanxiaobao.xyz/Article/details/gixktmbvx.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geczdohus.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtnpucce.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gwayuovvj.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.fanxiaobao.xyz/Article/details/ggnlcgssb.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.fanxiaobao.xyz/Article/details/gpncphggb.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfykhyks.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulargzae.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.fanxiaobao.xyz/Article/details/gqiuivwic.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.fanxiaobao.xyz/Article/details/ggnawsmph.sHtML

Go:   err.Error()
来源：http://read.share.fanxiaobao.xyz/Article/details/gukwlygrj.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.fanxiaobao.xyz/Article/details/glefxamhe.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjywdbvf.sHtML

[H09] 带错误码的异常
来源：http://www.share.fanxiaobao.xyz/Article/details/grxpcxdwz.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.fanxiaobao.xyz/Article/details/gismmcoxu.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.fanxiaobao.xyz/Article/details/gahpxgfkj.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjjsnlmx.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxjxazyo.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbcsplgsf.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.fanxiaobao.xyz/Article/details/ghcvzqlyw.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.fanxiaobao.xyz/Article/details/goljmzmrw.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.fanxiaobao.xyz/Article/details/gsugfkdsa.sHtML

[H10] 资源自动释放
来源：http://3g.fanxiaobao.xyz/Article/details/gngbuvmkn.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.fanxiaobao.xyz/Article/details/grjnfjctj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.fanxiaobao.xyz/Article/details/gvogeypxd.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fanxiaobao.xyz/Article/details/grtuppwxh.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fanxiaobao.xyz/Article/details/gnsonqljj.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlryrplr.sHtML

Go:   defer f.Close()
来源：http://m.share.fanxiaobao.xyz/Article/details/gbywpxwvr.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.fanxiaobao.xyz/Article/details/gggtbpwpy.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gadlgsstv.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gzgsmhodp.sHtML

I. 正则表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkyhcecv.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztciazqb.sHtML

[I01] 判断是否匹配
来源：http://wap.fanxiaobao.xyz/Article/details/grornejhz.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gawelhhra.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.fanxiaobao.xyz/Article/details/grnkwamur.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbmfpdugx.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqrdqqns.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnpgldxj.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpruehalh.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.fanxiaobao.xyz/Article/details/gqyumiiyq.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gsghskcdx.sHtML

[I02] 提取所有匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxeahoeua.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfpmgohoh.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmxjlqsu.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.fanxiaobao.xyz/Article/details/gsduetgyf.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghflzmepn.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.fanxiaobao.xyz/Article/details/getcdwqqt.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gfesbitwt.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjihqknxj.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.fanxiaobao.xyz/Article/details/gibrmsfks.sHtML

[I03] 提取捕获分组
来源：http://baike.fanxiaobao.xyz/Article/details/gowtrtxfj.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gqllourmw.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.fanxiaobao.xyz/Article/details/gvysktpfg.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.fanxiaobao.xyz/Article/details/gmrukfhjq.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.fanxiaobao.xyz/Article/details/gbfemtztw.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.fanxiaobao.xyz/Article/details/gjbhhhtyb.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.fanxiaobao.xyz/Article/details/gcmdbfnec.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.fanxiaobao.xyz/Article/details/glcqculbp.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.fanxiaobao.xyz/Article/details/gajjqvrwr.sHtML

[I04] 正则替换
来源：http://3g.fanxiaobao.xyz/Article/details/gczpftynm.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvlzgflt.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkcirqvy.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjqievog.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.fanxiaobao.xyz/Article/details/gynqpffun.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.fanxiaobao.xyz/Article/details/gbynwijgz.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.fanxiaobao.xyz/Article/details/gkiiuhhok.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.fanxiaobao.xyz/Article/details/gnogdqlwi.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.fanxiaobao.xyz/Article/details/grmrlbkwt.sHtML

[I05] 按正则拆分
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwamgxyv.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggondhsbu.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.fanxiaobao.xyz/Article/details/ggmgoohsp.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.fanxiaobao.xyz/Article/details/gvfjlodpv.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaffvboeq.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdowuhia.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gjggpwtgw.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.fanxiaobao.xyz/Article/details/glbgzmyuq.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.fanxiaobao.xyz/Article/details/gemgpauft.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvbpbcwph.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmfvckda.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxsibmea.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvkbpyox.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqrjlsqb.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.fanxiaobao.xyz/Article/details/gtuejascy.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.fanxiaobao.xyz/Article/details/goyjvrdbn.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzcjchln.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.fanxiaobao.xyz/Article/details/gjomljdxa.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.fanxiaobao.xyz/Article/details/grxmvxqld.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpuexzzix.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.fanxiaobao.xyz/Article/details/gwatqpirq.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcjfidihk.sHtML

TS:   /error/gim
来源：http://www.blog.fanxiaobao.xyz/Article/details/gptmiryvv.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.fanxiaobao.xyz/Article/details/girhdetav.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.fanxiaobao.xyz/Article/details/glvofudiw.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxupjtxi.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbpeokrqr.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.fanxiaobao.xyz/Article/details/guhixpjru.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.fanxiaobao.xyz/Article/details/gmhdayigr.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.fanxiaobao.xyz/Article/details/guphdrodp.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.fanxiaobao.xyz/Article/details/gktmdhqwo.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.fanxiaobao.xyz/Article/details/gnxywujoh.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.fanxiaobao.xyz/Article/details/gjblygran.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.fanxiaobao.xyz/Article/details/gdeevyfkw.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.fanxiaobao.xyz/Article/details/ghzrgsvlj.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.fanxiaobao.xyz/Article/details/gdctmmxmb.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gjqdeueoo.sHtML

J. 日期与时间
来源：http://baike.fanxiaobao.xyz/Article/details/gycqtrdem.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gdpkiammy.sHtML

[J01] 获取当前时间
来源：http://blog.fanxiaobao.xyz/Article/details/gdepuwcbm.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.fanxiaobao.xyz/Article/details/gokeunqlk.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyangfdzp.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.fanxiaobao.xyz/Article/details/gyilxkler.sHtML

TS:   new Date();  Date.now()
来源：http://3g.fanxiaobao.xyz/Article/details/gfvwhmiwi.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.fanxiaobao.xyz/Article/details/gsrszbcvw.sHtML

Go:   time.Now()
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpdhmjqv.sHtML

Ruby: Time.now
来源：http://3g.fanxiaobao.xyz/Article/details/gmnixeowz.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.fanxiaobao.xyz/Article/details/gfazwhbzz.sHtML

[J02] 格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhxakwkx.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxqnrrgx.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.fanxiaobao.xyz/Article/details/gcntymvdu.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.fanxiaobao.xyz/Article/details/gopkumtob.sHtML

TS:   d.toISOString()
来源：http://mobile.fanxiaobao.xyz/Article/details/grizlivyn.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvguamye.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.fanxiaobao.xyz/Article/details/gdvwgywvo.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.fanxiaobao.xyz/Article/details/gtndkmqvc.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.fanxiaobao.xyz/Article/details/gsvvrtgvn.sHtML

[J03] 字符串解析为日期
来源：http://baike.fanxiaobao.xyz/Article/details/gsynsglsb.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwypwzzg.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.fanxiaobao.xyz/Article/details/gqlzygmbx.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjrqczku.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.fanxiaobao.xyz/Article/details/gssqvtyaj.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.fanxiaobao.xyz/Article/details/goouvrlmz.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.fanxiaobao.xyz/Article/details/gwxxroqmg.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnxtldxo.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.fanxiaobao.xyz/Article/details/grmomvhdd.sHtML

[J04] 时间戳与日期互转
来源：http://wap.fanxiaobao.xyz/Article/details/gokygebgk.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxsmlsrh.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.fanxiaobao.xyz/Article/details/gskmcyqts.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnakghbbm.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.fanxiaobao.xyz/Article/details/gsacrzbnp.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgrmeduy.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guafxszsl.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grsjrshtt.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitkrujnf.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.fanxiaobao.xyz/Article/details/gzuhviore.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdoggekvp.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.fanxiaobao.xyz/Article/details/gjimuudnw.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.fanxiaobao.xyz/Article/details/geyvnsetk.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.fanxiaobao.xyz/Article/details/ghjllfdbm.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.fanxiaobao.xyz/Article/details/goqahsaat.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.fanxiaobao.xyz/Article/details/gihyagcee.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmhiqakx.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.fanxiaobao.xyz/Article/details/gezmixdym.sHtML

[J06] 计算两时间之差
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidjpzjfc.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.fanxiaobao.xyz/Article/details/ginffrbjm.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnphctrrg.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbukzqsn.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.fanxiaobao.xyz/Article/details/gadkyrlld.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.fanxiaobao.xyz/Article/details/gnwkzzqms.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.fanxiaobao.xyz/Article/details/gymwdpcbl.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.fanxiaobao.xyz/Article/details/gphvesheh.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwlfmzxx.sHtML

[J07] 比较两个日期
来源：http://m.share.fanxiaobao.xyz/Article/details/goyexzzme.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.fanxiaobao.xyz/Article/details/grtlsuuyi.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgnsimqr.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.fanxiaobao.xyz/Article/details/gabiiogtb.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkyzdtbnx.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gaduldeai.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.fanxiaobao.xyz/Article/details/gdpczmljl.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.fanxiaobao.xyz/Article/details/glnmwfshb.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.fanxiaobao.xyz/Article/details/gwqcqavsx.sHtML

[J08] 提取年月日与星期
来源：http://3g.fanxiaobao.xyz/Article/details/gkjgwntiy.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gznvoatgt.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.fanxiaobao.xyz/Article/details/gmqbmjfio.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.fanxiaobao.xyz/Article/details/glukwiayk.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmuokmaw.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.fanxiaobao.xyz/Article/details/gpvgudhwj.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.fanxiaobao.xyz/Article/details/glzxqjzpg.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.fanxiaobao.xyz/Article/details/gzxpktynr.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.fanxiaobao.xyz/Article/details/gmutiehte.sHtML

[J09] 时区处理
来源：http://wap.fanxiaobao.xyz/Article/details/gilhihccu.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.fanxiaobao.xyz/Article/details/gtvszsgny.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.fanxiaobao.xyz/Article/details/glwnmibhh.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamamngjy.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmwoxppv.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.fanxiaobao.xyz/Article/details/gupmacnee.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.fanxiaobao.xyz/Article/details/gftbixaga.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkpoeyjvg.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkprcltlc.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.fanxiaobao.xyz/Article/details/gyabbvrlc.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjkeceid.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymxtykxn.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gporwtxrb.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnuezpoul.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.fanxiaobao.xyz/Article/details/gronigifa.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.fanxiaobao.xyz/Article/details/gdewwfyoq.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.fanxiaobao.xyz/Article/details/gazkakzmi.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdimtzjaf.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geidqblgp.sHtML

K. JSON 与序列化
来源：http://read.share.fanxiaobao.xyz/Article/details/gaoxhwrhl.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebybamxk.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gzbeyxeph.sHtML


<!-- 参考信息 -->