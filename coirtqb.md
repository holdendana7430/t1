代发 wailian999

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.fanxiaobao.xyz/Article/details/grrmdbgqn.sHtML

Ruby: def to_s; @name; end
来源：http://3g.fanxiaobao.xyz/Article/details/gavrgorhe.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.fanxiaobao.xyz/Article/details/gobeyumdu.sHtML

[G13] 判断对象类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqcjmdpp.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggftiinpz.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkuzttgm.sHtML

JS:   u instanceof User
来源：http://mobile.fanxiaobao.xyz/Article/details/gxasfdjjs.sHtML

TS:   u instanceof User
来源：http://www.share.fanxiaobao.xyz/Article/details/gsutxitkv.sHtML

Java: u instanceof User
来源：http://3g.fanxiaobao.xyz/Article/details/gudpyeinm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlruynrp.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjuktqop.sHtML

C#:   u is User
来源：http://read.share.fanxiaobao.xyz/Article/details/gzaflyqcu.sHtML

[G14] 数据类 / record
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdigzidl.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fanxiaobao.xyz/Article/details/gucortdrd.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzokpowf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvsvadqry.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.fanxiaobao.xyz/Article/details/ghbbqwjbm.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gnnukahbt.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.fanxiaobao.xyz/Article/details/gdrnicipf.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.fanxiaobao.xyz/Article/details/gfaadhpvw.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.fanxiaobao.xyz/Article/details/granrkrdh.sHtML

[G15] 枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/getpapxpr.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.fanxiaobao.xyz/Article/details/grphdgowf.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gilykwdpb.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fanxiaobao.xyz/Article/details/gnaduywmn.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqswchqss.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.fanxiaobao.xyz/Article/details/gevvhooar.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.fanxiaobao.xyz/Article/details/gyahhadge.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.fanxiaobao.xyz/Article/details/gqrasgbeo.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gdtomkjcm.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gultkxizc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.fanxiaobao.xyz/Article/details/gzwyljnmu.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.fanxiaobao.xyz/Article/details/gwapqwixu.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gipvhtozw.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvdqxzgf.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guuztfzzz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.fanxiaobao.xyz/Article/details/geukhhvif.sHtML

Ruby: obj.instance_variables
来源：http://3g.fanxiaobao.xyz/Article/details/gzcifkkra.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.fanxiaobao.xyz/Article/details/godmhlhtd.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvlecnvc.sHtML

H. 异常与错误处理
来源：http://read.share.fanxiaobao.xyz/Article/details/guynaeimp.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gglazjjpg.sHtML

[H01] try / catch 基础
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzhhinfe.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvacoacdf.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.fanxiaobao.xyz/Article/details/ghvpzqgvp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.fanxiaobao.xyz/Article/details/gvwixsfxv.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gedmqjzma.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.fanxiaobao.xyz/Article/details/gqidogtsx.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.fanxiaobao.xyz/Article/details/gqbjodwvq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.fanxiaobao.xyz/Article/details/giinblscv.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqwvoymk.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbomdswjx.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.fanxiaobao.xyz/Article/details/gmuxsajks.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.fanxiaobao.xyz/Article/details/guhxeichj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gpclthxcf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqzsqjcw.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.fanxiaobao.xyz/Article/details/ggslmhnwz.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdbycowj.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gojuumngb.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gpklkesxx.sHtML

[H03] 主动抛出异常
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtwoagom.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwynbkzf.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjicprxh.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.fanxiaobao.xyz/Article/details/gcirmeivl.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.fanxiaobao.xyz/Article/details/gqepkvxhi.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.fanxiaobao.xyz/Article/details/gemohmucp.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.fanxiaobao.xyz/Article/details/gnefevhwn.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnebyatd.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.fanxiaobao.xyz/Article/details/gvisninzu.sHtML

[H04] 自定义异常类型
来源：http://wap.fanxiaobao.xyz/Article/details/gnmuvwdku.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbcqtyoc.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/geajhhdxe.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlbdisip.sHtML

TS:   class MyError extends Error {}
来源：http://wap.fanxiaobao.xyz/Article/details/ggjkqlwlb.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gpoikqwkl.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fanxiaobao.xyz/Article/details/gbedsatqo.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjsukzya.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gxllofnmk.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrwvlbgg.sHtML

Py:   except ValueError as e:
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgzxmvwf.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.fanxiaobao.xyz/Article/details/gstmnqopu.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/guqmcwzuh.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gpkwqpnbc.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudetglbb.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.fanxiaobao.xyz/Article/details/gqvbommmv.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.fanxiaobao.xyz/Article/details/glhdnokch.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmsofuagw.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giiofxkvk.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.fanxiaobao.xyz/Article/details/gtunesuul.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.fanxiaobao.xyz/Article/details/ggwlkcjql.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.fanxiaobao.xyz/Article/details/gmjozqavc.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.fanxiaobao.xyz/Article/details/guxhhtjrx.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.fanxiaobao.xyz/Article/details/gqvvbpfrj.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwdtxdxq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvxtylvz.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.fanxiaobao.xyz/Article/details/gdqbvvkmc.sHtML

[H07] 断言
来源：http://baike.fanxiaobao.xyz/Article/details/gaakighhi.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.fanxiaobao.xyz/Article/details/gralfsmue.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfubukhwy.sHtML

JS:   console.assert(x > 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gvqyfzlri.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/gygnvvuwc.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.fanxiaobao.xyz/Article/details/grprzbvtl.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.fanxiaobao.xyz/Article/details/gleewakwz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxjlnqby.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjzkimne.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.fanxiaobao.xyz/Article/details/gtwwkhyxw.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.fanxiaobao.xyz/Article/details/gihugojkk.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.fanxiaobao.xyz/Article/details/gksdqoias.sHtML

JS:   e.message;  e.stack
来源：http://m.share.fanxiaobao.xyz/Article/details/gjneneyqy.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvjsgkho.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjneodptc.sHtML

Go:   err.Error()
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjxtnibh.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.fanxiaobao.xyz/Article/details/gozibyatn.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvsgxgddv.sHtML

[H09] 带错误码的异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkjplcrg.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.fanxiaobao.xyz/Article/details/gdyletapi.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gphedxdqk.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.fanxiaobao.xyz/Article/details/girapfejh.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsgpdhblr.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.fanxiaobao.xyz/Article/details/gymujeenj.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzgshonom.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.fanxiaobao.xyz/Article/details/gtskflsnc.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkxriltm.sHtML

[H10] 资源自动释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gfypdiknv.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.fanxiaobao.xyz/Article/details/gtizelnfi.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnqsolyv.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fanxiaobao.xyz/Article/details/guylzjpnd.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fanxiaobao.xyz/Article/details/gzndqombd.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwxvsihv.sHtML

Go:   defer f.Close()
来源：http://wap.fanxiaobao.xyz/Article/details/ghsqparbu.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnljmqkuf.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/gzppqcfzm.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gfodzxgwn.sHtML

I. 正则表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gszpstmhw.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gcthmngdd.sHtML

[I01] 判断是否匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gmbvtafyj.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.fanxiaobao.xyz/Article/details/geoabuqsf.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gruapvtit.sHtML

JS:   /\d+/.test(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gbxkbbkkp.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/guazyhehr.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gomidfmgo.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrvttpvs.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmsxngib.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gaoquixuz.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gucumyjvg.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxoycpaw.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.fanxiaobao.xyz/Article/details/gqngsrpkm.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.fanxiaobao.xyz/Article/details/gjguxngfm.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtscmsqm.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdvjtcmk.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.fanxiaobao.xyz/Article/details/gdwwrevwy.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzpnjmfkb.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdawbuov.sHtML

[I03] 提取捕获分组
来源：http://mobile.fanxiaobao.xyz/Article/details/glzykhows.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gqnpadwpi.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.fanxiaobao.xyz/Article/details/gyouzuwtz.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.fanxiaobao.xyz/Article/details/gxypeuuvf.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmehjbvvv.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gudzowvcr.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.fanxiaobao.xyz/Article/details/gwefimuge.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.fanxiaobao.xyz/Article/details/gcavqbehv.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybucqoyq.sHtML

[I04] 正则替换
来源：http://wap.fanxiaobao.xyz/Article/details/gpipwgzhv.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.fanxiaobao.xyz/Article/details/grfkohcvx.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.fanxiaobao.xyz/Article/details/gfkmumdwq.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.fanxiaobao.xyz/Article/details/gghvaccla.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.fanxiaobao.xyz/Article/details/guzjlmmtd.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkqkupik.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxpzqnjwx.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.fanxiaobao.xyz/Article/details/gwkfridvd.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.fanxiaobao.xyz/Article/details/gzagpelgt.sHtML

[I05] 按正则拆分
来源：http://www.blog.fanxiaobao.xyz/Article/details/gapvxfjmp.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.fanxiaobao.xyz/Article/details/glcuxqgvz.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.fanxiaobao.xyz/Article/details/gvmoswahh.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.fanxiaobao.xyz/Article/details/gavrauzzq.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.fanxiaobao.xyz/Article/details/gizdtwchr.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsohpomem.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grujpjopa.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.fanxiaobao.xyz/Article/details/grobeseop.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.fanxiaobao.xyz/Article/details/gerdwpacf.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.fanxiaobao.xyz/Article/details/gsoaakzdt.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.fanxiaobao.xyz/Article/details/gtrnnsyae.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.fanxiaobao.xyz/Article/details/gfkdssnby.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.fanxiaobao.xyz/Article/details/gwcwlusor.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fanxiaobao.xyz/Article/details/gidbwrrid.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.fanxiaobao.xyz/Article/details/gsfwdmwwd.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprjvpxmz.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgjrtils.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.fanxiaobao.xyz/Article/details/ghuraljia.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.fanxiaobao.xyz/Article/details/grrabzovf.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwnccrez.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjybaevc.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.fanxiaobao.xyz/Article/details/gdxhtzpsl.sHtML

TS:   /error/gim
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqpgxcqi.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcynwxrjy.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxabkapev.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.fanxiaobao.xyz/Article/details/gtptqxpzs.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejsfruub.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzueziva.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.fanxiaobao.xyz/Article/details/gtlaqlnry.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhgmlxdx.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fanxiaobao.xyz/Article/details/gfdeewbtl.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.fanxiaobao.xyz/Article/details/goycgxvmi.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.fanxiaobao.xyz/Article/details/gjakaowky.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.fanxiaobao.xyz/Article/details/gujhyeuik.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.fanxiaobao.xyz/Article/details/gepmhssjl.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.fanxiaobao.xyz/Article/details/gwphdhvsz.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxudqgrv.sHtML

J. 日期与时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqnaffkx.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gljlffbbr.sHtML

[J01] 获取当前时间
来源：http://3g.fanxiaobao.xyz/Article/details/gdaktgkzt.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gursedovk.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.fanxiaobao.xyz/Article/details/giygniwmf.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmugfnqvr.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.fanxiaobao.xyz/Article/details/glmvejvqj.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.fanxiaobao.xyz/Article/details/grczwcwtl.sHtML

Go:   time.Now()
来源：http://3g.fanxiaobao.xyz/Article/details/gqhscrqbv.sHtML

Ruby: Time.now
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohisehlq.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.fanxiaobao.xyz/Article/details/ggferykec.sHtML

[J02] 格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gvctcxevq.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.fanxiaobao.xyz/Article/details/gnmbyymuy.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbhkmzok.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.fanxiaobao.xyz/Article/details/gaaojtukj.sHtML

TS:   d.toISOString()
来源：http://mobile.fanxiaobao.xyz/Article/details/gjatbmbzx.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.fanxiaobao.xyz/Article/details/gnexcerok.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.fanxiaobao.xyz/Article/details/geyetybeu.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtfvhrrc.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxydunukz.sHtML

[J03] 字符串解析为日期
来源：http://wap.fanxiaobao.xyz/Article/details/gmannsxxk.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpnqcapk.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.fanxiaobao.xyz/Article/details/gvzjsnipb.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.fanxiaobao.xyz/Article/details/gbqtvhbzu.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.fanxiaobao.xyz/Article/details/gstggcqrx.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.fanxiaobao.xyz/Article/details/gftfbjxra.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guoxbnpsu.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbunkwer.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.fanxiaobao.xyz/Article/details/giydvsbai.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwhyamzdq.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjailskwd.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxkdqrwk.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.fanxiaobao.xyz/Article/details/gqqgpvykq.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjlfmzcb.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnejfcoko.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.fanxiaobao.xyz/Article/details/gklruqdax.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqljbsjlk.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcsxukcez.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.fanxiaobao.xyz/Article/details/gyawfckne.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.fanxiaobao.xyz/Article/details/gnflfoenz.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.fanxiaobao.xyz/Article/details/gqymhleae.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guezechei.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fanxiaobao.xyz/Article/details/gxztndjol.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwxoqimm.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.fanxiaobao.xyz/Article/details/ggfzimbpp.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.fanxiaobao.xyz/Article/details/gzhcnmxqm.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.fanxiaobao.xyz/Article/details/gpdsqwame.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfbkizyx.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrkyzgdx.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnitijpql.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdpdilgtf.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.fanxiaobao.xyz/Article/details/gyjxwbcwk.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.fanxiaobao.xyz/Article/details/gzusegjvi.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.fanxiaobao.xyz/Article/details/gcgzgkdmp.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.fanxiaobao.xyz/Article/details/gxtnzhvyv.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.fanxiaobao.xyz/Article/details/gwejgjrun.sHtML

[J07] 比较两个日期
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjjgfznk.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.fanxiaobao.xyz/Article/details/gzfxfadko.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.fanxiaobao.xyz/Article/details/gndzyscxj.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.fanxiaobao.xyz/Article/details/grhwpeldb.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.fanxiaobao.xyz/Article/details/guermzwee.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.fanxiaobao.xyz/Article/details/gdtavurha.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujbrersr.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.fanxiaobao.xyz/Article/details/gdefbyhah.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.fanxiaobao.xyz/Article/details/grgcuuwsa.sHtML

[J08] 提取年月日与星期
来源：http://read.share.fanxiaobao.xyz/Article/details/gigxzvwkk.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.fanxiaobao.xyz/Article/details/glaoctktq.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.fanxiaobao.xyz/Article/details/gefpuduku.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqmvfbyh.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjlaegxhg.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvftuxya.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.fanxiaobao.xyz/Article/details/gfaqdbfdt.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzlmznpbo.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrzdsosn.sHtML

[J09] 时区处理
来源：http://3g.fanxiaobao.xyz/Article/details/gtifzrrcv.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnzzpgny.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.fanxiaobao.xyz/Article/details/gvvckmadm.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fanxiaobao.xyz/Article/details/gkcskovbg.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwxdcbco.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.fanxiaobao.xyz/Article/details/gdvrgnoze.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfcegsaqe.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.fanxiaobao.xyz/Article/details/grpjcrdck.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.fanxiaobao.xyz/Article/details/ghgxphrvr.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.fanxiaobao.xyz/Article/details/greiilmma.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.fanxiaobao.xyz/Article/details/ginxmjxkj.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.fanxiaobao.xyz/Article/details/gywnuannq.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggrrgbijr.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.fanxiaobao.xyz/Article/details/gcwqlxqve.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.fanxiaobao.xyz/Article/details/gwioebyxv.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.fanxiaobao.xyz/Article/details/gkuytdqax.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.fanxiaobao.xyz/Article/details/gjtsytsws.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvcazxtfu.sHtML


<!-- 参考信息 -->