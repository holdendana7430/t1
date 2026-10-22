代发 wailian999

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2sxhadnfl.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2msgkwaog.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2jtvlshhb.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2khyrvthp.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2emdmjurb.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2stlsazdw.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2rlgudxer.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2xxnjmktf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2pwxewwut.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2runiyqhw.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2tmzuhszb.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2wgoyxbmc.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2faitxwav.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ggrcbwqz.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2gttlixfu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2dfsdqsto.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2wwranmnz.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2mwdidstf.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rekjxxbb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2kzfxcbpz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2vgfnrdnq.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2isfzojyc.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2fxsqdcst.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jrpsaoab.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2gphkydqu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xgmyighs.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2qouhynaf.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2mdxhgghk.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2hwehslbc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2yxvwggax.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2arvlcgxh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2uzwaiyla.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2gsgiffyk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2caqnktmo.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2btugukgj.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2kbyavagj.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2ogvpfklz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yalfmzri.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ntzykwlq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ckkwocdo.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2eeobsiax.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2mdiyrtep.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2wlehtpun.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bjhgyiew.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2bddwvbcw.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2wqcibooj.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2wtqojkfu.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2loojfnsu.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2feyyzori.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2hteyyotd.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2zdgjqhbo.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2eztrlqch.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2embmayhg.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2ijdpacdf.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2zojfrheo.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2gxfyhayv.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2pmkbgjri.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2gxtmpxsj.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ghdksrtp.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2krmgdplj.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2paefvylw.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2ofnrjmyj.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2ztpvyfmw.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2lfmqkwwe.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2sbgdcxrz.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2qdmpatfm.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2oeeoqsej.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vdruaxav.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2whgditha.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2qfapsrrj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bitnioyy.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2untnrkjs.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2iywcpcwg.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2smkihhbr.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2bwpzfous.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2fldehdvq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2qzirubfx.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2osqfktkl.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2adqdqwqz.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2spdjodms.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2qfredxrw.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2twzndqdx.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2jjpfwbpx.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2pfodupvm.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pghawgse.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2futcjajc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2oyjxbnqs.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2alndkqot.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2vaxnuisj.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2jzqnzqkl.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2oavlcnpe.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2eeunhhla.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2fqstdlba.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2ydeaercb.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2utewentq.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2ctxephvv.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2dridqnco.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2dharxozm.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2sdkfefvx.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2crqklcwa.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2rhsipyfn.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2pyqebzgc.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2iqvwgjpc.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2bsrhittv.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2mbudqmij.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2pnpteaqj.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2bmdldaun.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2itnrrvwc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2sdbkkmtk.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2rwzueyhb.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2dgxwubmd.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2vjzkmeie.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2frdijthg.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2shjppmkm.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2gahjvvsk.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2eyxlhbaf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hgerpeyp.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2gctllnfp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qdqjbgmz.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2nqomcheb.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2xihhzint.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2eokftdka.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2uokauvji.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yfbestul.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2rrnrcgkk.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2dzsftyrv.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2iknlwiig.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2cmwghiyi.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2encgfuui.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2juecpwvi.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2hcbgzmye.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2gfwqbchc.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2gktupslb.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2migdmabg.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2qucyxhbn.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ltndxlhz.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2odfxuiqi.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2qzpigqcf.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2btrnhlyt.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2cfcghzsr.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2toesmmcx.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2vysmxyfg.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2nvkvcyre.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2tltvizse.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2jeuygvhr.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2fkylwwvy.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2undpovte.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2epefgxpn.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2llvntizc.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2thkwibqy.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2uthccgxg.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2pwztoswh.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2blctxtir.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2slvvsvgp.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2avebgfxt.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2hahxegum.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2fdsrtndx.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2rafzuanz.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2jmdugpyo.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2ygjicmdq.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2poyuanph.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ihhhesyc.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2yeuvhqha.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2mnqflhzs.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2lrvlruhg.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2usfcjxon.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2lajsqegn.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2gvigfwha.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2acaebihp.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2ektmsbjf.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2rsyvjlvv.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2fhiadxuj.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2geomzdbe.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2vxbmrpet.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2jujreyjf.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2tsklplmd.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2pnwxloqz.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2mgzjspmv.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2rerzhhwp.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2nyoiplax.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2djpsveea.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2ksegqbze.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2jgqfefom.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2mltcuijh.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2hqznntfr.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2bspgxtof.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2bbqqvmfh.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2merndyfv.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2kpponhdb.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2akwuwtdc.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2apxwspej.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qevbzvps.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2wczvnqxj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dhfulklb.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2stqjfyza.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2zlvqmbef.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2sjbojtwm.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2btyvclgc.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2ukftxbfk.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2mkfxzzta.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2tdzhsfql.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2azssuybj.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2ifickxkx.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2vluoalyf.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2jdyjawtr.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2lpbeezma.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2skudnifv.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2nrwednlo.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2iylfsvav.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2ekbzntwp.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2mgekicae.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2uuqqeltr.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2iwoukzot.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2wpdxypwc.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2nhisatii.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2oashaqgw.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2arowdxrh.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2eyonvoat.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2tlkmszte.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2mkneyetp.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2wblqcorv.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2imvsphfr.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2tpctkeni.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2joawqmgh.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2yfpftjki.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2pwwsoapy.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2uitqwfwt.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2qfxnycpz.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2qomihels.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2ghdkelce.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2dfarafqx.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2sfghmgqo.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2rdbnxvud.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2dkuzxscg.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2nctcugum.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2jvlhuacj.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2okrziqgf.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2akyalzdk.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2jtrgpbli.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2vdfqajmg.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2nelpedjq.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2wiwmqtyb.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2ujxrxsrz.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2qxyjlshi.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2keqzztyd.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2ustfmyxj.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2liwwgvdb.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2hbnyrypb.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2ptpywiay.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2owlrvolh.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2tpeygted.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2pjfjbyiu.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2ftclwbny.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2mookdkhf.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2aozoyaav.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2uwikxifv.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2ivdxoonz.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2wmedcvqb.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2fzlyezuw.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2nsdbbcfz.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2fynblzmj.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2gkhmguoh.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2ucvxodyo.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2gnlvsfvp.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2wqdilqfu.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2kaipvasv.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2aokrazyk.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2zvyfkoeu.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2yswzzlvh.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2ykaviyyi.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2bjlqxqmj.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2sjgbzypz.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2ryrcyhwr.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2ogtfkdvs.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2ofvgbgcv.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2vwnpkuyj.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2ugydvwud.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2nforhdtc.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2iahvnfvn.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2twqvzojj.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mamoxovq.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2vxigorcm.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2pfarfotb.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dtstcwzy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bwhsydro.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2phzkespj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xkwxozkr.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kmmfkriy.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2mkjkotoh.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2xqpyrhtp.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nobpdhbs.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2jfftllls.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2rwyctczm.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2hogjebyw.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2qqgvpvfk.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rrivewif.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2dymbrdhx.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2jyhpoyst.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2vcmppukl.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2llvnamkk.html


<!-- 参考信息 -->