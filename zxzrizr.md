代发 wailian999

[G14] 数据类 / record
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpxhykzb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.fanxiaobao.xyz/Article/details/gpqfuqgga.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.fanxiaobao.xyz/Article/details/gejoczffz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.fanxiaobao.xyz/Article/details/geoatuxfr.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.fanxiaobao.xyz/Article/details/gamikvyvv.sHtML

Java: record User(String name, int age) {}
来源：http://baike.fanxiaobao.xyz/Article/details/glziuolss.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.fanxiaobao.xyz/Article/details/gppjnigfs.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.fanxiaobao.xyz/Article/details/gdnvsfsti.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdazwhkt.sHtML

[G15] 枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gwyvduvta.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fanxiaobao.xyz/Article/details/gzqpcihdu.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gzlzcdmqf.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fanxiaobao.xyz/Article/details/gunnqrhua.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/goyswnehm.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxurmkvy.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxghjwlgt.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.fanxiaobao.xyz/Article/details/gwkhotbdt.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/griotaoxp.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwnykpqa.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.fanxiaobao.xyz/Article/details/gbptamslg.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.fanxiaobao.xyz/Article/details/guycaxmgb.sHtML

JS:   Object.entries(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gmglgmdbe.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjthgknmg.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjsiwxrtq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.fanxiaobao.xyz/Article/details/gacnfcsxw.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbliwtqlo.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.fanxiaobao.xyz/Article/details/gzsoraysa.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzkuupufa.sHtML

H. 异常与错误处理
来源：http://wap.fanxiaobao.xyz/Article/details/gtvzqyhlj.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefvszvia.sHtML

[H01] try / catch 基础
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjshgdsa.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.fanxiaobao.xyz/Article/details/gqxxtnvwv.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gjyqjihia.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqyhcztc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.fanxiaobao.xyz/Article/details/gjhighoju.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gifrsbmmp.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/grydjettz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatkjzdvm.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpnrzjay.sHtML

[H02] finally / ensure 收尾
来源：http://blog.fanxiaobao.xyz/Article/details/gomxovovf.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.fanxiaobao.xyz/Article/details/gueknixwi.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdpzcwqr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gafuqntso.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgfuczvh.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdccwxirg.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.fanxiaobao.xyz/Article/details/gopxpxflc.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.fanxiaobao.xyz/Article/details/glonukgwk.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtysxjvob.sHtML

[H03] 主动抛出异常
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxogqgok.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.fanxiaobao.xyz/Article/details/guktvcfhg.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.fanxiaobao.xyz/Article/details/gpiauymby.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.fanxiaobao.xyz/Article/details/gqbmncdyk.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.fanxiaobao.xyz/Article/details/gbxitxxyy.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkapdlal.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggziyeseh.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.fanxiaobao.xyz/Article/details/gasyhveri.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmscvqxa.sHtML

[H04] 自定义异常类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkdpzcpe.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqcluqma.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjmcrhqa.sHtML

JS:   class MyError extends Error {}
来源：http://blog.fanxiaobao.xyz/Article/details/gmtpietoj.sHtML

TS:   class MyError extends Error {}
来源：http://wap.fanxiaobao.xyz/Article/details/gaesyrjvy.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gldosmgzz.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghgsfuiaw.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gvcsjglou.sHtML

C#:   class MyException : Exception {}
来源：http://3g.fanxiaobao.xyz/Article/details/geoexeoyz.sHtML

[H05] 捕获特定类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gjisqztfe.sHtML

Py:   except ValueError as e:
来源：http://www.share.fanxiaobao.xyz/Article/details/ghupkasgw.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgsrfxij.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.fanxiaobao.xyz/Article/details/ggvbpmlgh.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gfgehtuju.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnfwpwzz.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmkvhhwab.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.fanxiaobao.xyz/Article/details/geqmsbvlg.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmtocibl.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.fanxiaobao.xyz/Article/details/gsppsregv.sHtML

Py:   value = d.get("k") or default
来源：http://3g.fanxiaobao.xyz/Article/details/grzbaqvtl.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhsoryxf.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtuaxwsl.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxzlyrhf.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.fanxiaobao.xyz/Article/details/grcxlhjxn.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.fanxiaobao.xyz/Article/details/gqovnvtob.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdzsnvve.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.fanxiaobao.xyz/Article/details/gcejymwyp.sHtML

[H07] 断言
来源：http://3g.fanxiaobao.xyz/Article/details/gialbydrh.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.fanxiaobao.xyz/Article/details/glegcucax.sHtML

PHP:  assert($x > 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggofkldwt.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggrhzfwgo.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukmjufal.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.fanxiaobao.xyz/Article/details/gwncvouuf.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijcaleon.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.fanxiaobao.xyz/Article/details/ghloqutxf.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gwyhkeubf.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.fanxiaobao.xyz/Article/details/grjmgbomt.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.fanxiaobao.xyz/Article/details/gottcehlc.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.fanxiaobao.xyz/Article/details/guuqfmfup.sHtML

JS:   e.message;  e.stack
来源：http://3g.fanxiaobao.xyz/Article/details/gfordurad.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.fanxiaobao.xyz/Article/details/gradygmih.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.fanxiaobao.xyz/Article/details/gjyrynlnv.sHtML

Go:   err.Error()
来源：http://baike.fanxiaobao.xyz/Article/details/giqqswwbz.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.fanxiaobao.xyz/Article/details/gwepzuzbu.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.fanxiaobao.xyz/Article/details/gdvbcwhwx.sHtML

[H09] 带错误码的异常
来源：http://baike.fanxiaobao.xyz/Article/details/geujkerof.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkjolqgs.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.fanxiaobao.xyz/Article/details/gknslnkfi.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.fanxiaobao.xyz/Article/details/glpyrflkq.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjsvjxgll.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.fanxiaobao.xyz/Article/details/gwydecjgi.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gusohiiop.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbipfnngo.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.fanxiaobao.xyz/Article/details/gspddxidw.sHtML

[H10] 资源自动释放
来源：http://blog.fanxiaobao.xyz/Article/details/gbttucfbl.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.fanxiaobao.xyz/Article/details/guwmmkxgk.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.fanxiaobao.xyz/Article/details/glzyufxhj.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvpiqnfk.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fanxiaobao.xyz/Article/details/gruewocji.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzcuxqtz.sHtML

Go:   defer f.Close()
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwmsgbni.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.fanxiaobao.xyz/Article/details/grsnalnjp.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glugugsfi.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecyznhhd.sHtML

I. 正则表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gcgncsvek.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gnnxvwvry.sHtML

[I01] 判断是否匹配
来源：http://baike.fanxiaobao.xyz/Article/details/girkeatro.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzhftsio.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.fanxiaobao.xyz/Article/details/gstpuzatf.sHtML

JS:   /\d+/.test(s)
来源：http://baike.fanxiaobao.xyz/Article/details/grwlyhwfg.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpyxxfnuy.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllugvmuv.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqwxwjoj.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.fanxiaobao.xyz/Article/details/gkeqqqcpw.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.fanxiaobao.xyz/Article/details/gcpsetdjn.sHtML

[I02] 提取所有匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkfdekil.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmrcleap.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.fanxiaobao.xyz/Article/details/gqgcridls.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.fanxiaobao.xyz/Article/details/gxxxbvbxv.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.fanxiaobao.xyz/Article/details/gqmhoakzy.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvkxouji.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gngqitwtk.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.fanxiaobao.xyz/Article/details/gqtbgfzli.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjykoeez.sHtML

[I03] 提取捕获分组
来源：http://mobile.fanxiaobao.xyz/Article/details/gyacuiuka.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gsuvgymbe.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.fanxiaobao.xyz/Article/details/gpovfehbw.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfzsncdr.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.fanxiaobao.xyz/Article/details/guekajaer.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfocwnejg.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhpowfwz.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.fanxiaobao.xyz/Article/details/getgbjjdz.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcayduwfp.sHtML

[I04] 正则替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gprxlbrvi.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gveugfjxt.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.fanxiaobao.xyz/Article/details/gcfmgwjxd.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.fanxiaobao.xyz/Article/details/grxnoaxea.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.fanxiaobao.xyz/Article/details/godqjqsat.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfdtbmet.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.fanxiaobao.xyz/Article/details/gvlydfgep.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.fanxiaobao.xyz/Article/details/gjlgtfrft.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbpyvvwf.sHtML

[I05] 按正则拆分
来源：http://mobile.fanxiaobao.xyz/Article/details/glzlxjhyp.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gklcokofg.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqikbmjlj.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.fanxiaobao.xyz/Article/details/giyoodcpu.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.fanxiaobao.xyz/Article/details/grerwlnha.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcvfxnlv.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.fanxiaobao.xyz/Article/details/ghqrprgch.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.fanxiaobao.xyz/Article/details/gwtzjkfjw.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcicdrocz.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.fanxiaobao.xyz/Article/details/gxpnqujkq.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxrjyckv.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.fanxiaobao.xyz/Article/details/grbabyzgv.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbkbjtoaw.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.fanxiaobao.xyz/Article/details/gumyfpevz.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqxyeyaw.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.fanxiaobao.xyz/Article/details/gonyvsvwz.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqtcbsbs.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.fanxiaobao.xyz/Article/details/gamlfxnru.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtuhmfrp.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvltqotrf.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.fanxiaobao.xyz/Article/details/glkfzkkwv.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndnuqomk.sHtML

TS:   /error/gim
来源：http://3g.fanxiaobao.xyz/Article/details/gbmojibbp.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktxwbvgk.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.fanxiaobao.xyz/Article/details/gjmnmlqyo.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.fanxiaobao.xyz/Article/details/gszydeopc.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.fanxiaobao.xyz/Article/details/giqvccvtx.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.fanxiaobao.xyz/Article/details/glyhdwoln.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxiqdwnxd.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.fanxiaobao.xyz/Article/details/guceecuau.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmbbbbbb.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.fanxiaobao.xyz/Article/details/gnmitbqzf.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgchawfn.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.fanxiaobao.xyz/Article/details/gccbihknx.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.fanxiaobao.xyz/Article/details/gyedqlcxx.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giyrzhkus.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxnryklt.sHtML

J. 日期与时间
来源：http://wap.fanxiaobao.xyz/Article/details/goityurnw.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvdmjhhj.sHtML

[J01] 获取当前时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdhvsqck.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.fanxiaobao.xyz/Article/details/grfrtudim.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.fanxiaobao.xyz/Article/details/gnmjktrtx.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtlmdljdu.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.fanxiaobao.xyz/Article/details/gykaojzzk.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.fanxiaobao.xyz/Article/details/guwaeknrq.sHtML

Go:   time.Now()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcnmrvyfo.sHtML

Ruby: Time.now
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmckuipv.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.fanxiaobao.xyz/Article/details/gpucqhvtb.sHtML

[J02] 格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjlhepkd.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.fanxiaobao.xyz/Article/details/gjkgehvuk.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.fanxiaobao.xyz/Article/details/gfeufmays.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqwnmryax.sHtML

TS:   d.toISOString()
来源：http://www.share.fanxiaobao.xyz/Article/details/glgeaycjo.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqpcdubh.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.fanxiaobao.xyz/Article/details/gnobdmouu.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.fanxiaobao.xyz/Article/details/ggeehexki.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtroifjsq.sHtML

[J03] 字符串解析为日期
来源：http://blog.fanxiaobao.xyz/Article/details/ghktswosq.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.fanxiaobao.xyz/Article/details/gvshjyqkr.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.fanxiaobao.xyz/Article/details/grkqwzori.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmpypnuy.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.fanxiaobao.xyz/Article/details/ggukajpwx.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqkyykfg.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.fanxiaobao.xyz/Article/details/gqymiwzfz.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.fanxiaobao.xyz/Article/details/gtunqvsql.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.fanxiaobao.xyz/Article/details/grsnbhugo.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbzpettq.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.fanxiaobao.xyz/Article/details/gjrejepkd.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrnvxtcu.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkfwmlkv.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdppmofqm.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvfoxldxw.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.fanxiaobao.xyz/Article/details/ghhurvuqg.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.fanxiaobao.xyz/Article/details/gvuzdpznu.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.fanxiaobao.xyz/Article/details/glxeykeft.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.fanxiaobao.xyz/Article/details/gczxveqpk.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.fanxiaobao.xyz/Article/details/grkinzvkm.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.fanxiaobao.xyz/Article/details/gpqijicjx.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.fanxiaobao.xyz/Article/details/gecubmkkd.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.fanxiaobao.xyz/Article/details/gnvbmgtnz.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpycypruk.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guptjbwai.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.fanxiaobao.xyz/Article/details/gixvgtiwn.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.fanxiaobao.xyz/Article/details/gxbinluye.sHtML

[J06] 计算两时间之差
来源：http://wap.fanxiaobao.xyz/Article/details/gpmgepuow.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.fanxiaobao.xyz/Article/details/gdgdfqhgw.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.fanxiaobao.xyz/Article/details/ggexnexap.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtheuqlw.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.fanxiaobao.xyz/Article/details/ghyopybkl.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.fanxiaobao.xyz/Article/details/ggfkzvawx.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjfyffyd.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.fanxiaobao.xyz/Article/details/gtsfkhnea.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.fanxiaobao.xyz/Article/details/gragthlfz.sHtML

[J07] 比较两个日期
来源：http://wap.fanxiaobao.xyz/Article/details/gxkozeizm.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glosffhma.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.fanxiaobao.xyz/Article/details/gcrmedcmf.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwtfqwdq.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.fanxiaobao.xyz/Article/details/gscoxindw.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtypvkoag.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfhlnxqbw.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.fanxiaobao.xyz/Article/details/gzjcvqcxe.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldfavftd.sHtML

[J08] 提取年月日与星期
来源：http://3g.fanxiaobao.xyz/Article/details/gsxzlftpc.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.fanxiaobao.xyz/Article/details/gzbmkkszo.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.fanxiaobao.xyz/Article/details/goydsztrd.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.fanxiaobao.xyz/Article/details/gshatypdy.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqwyrhgo.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.fanxiaobao.xyz/Article/details/gfjqkjcjz.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.fanxiaobao.xyz/Article/details/gisfkaxoq.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.fanxiaobao.xyz/Article/details/gycejybzk.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqfmxrpk.sHtML

[J09] 时区处理
来源：http://wap.fanxiaobao.xyz/Article/details/gcbqwvkjg.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.fanxiaobao.xyz/Article/details/gflytrmfv.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndtatpem.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fanxiaobao.xyz/Article/details/gsxkeuyzu.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fanxiaobao.xyz/Article/details/gdxgbpvcd.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.fanxiaobao.xyz/Article/details/gehuvtqhy.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpaymfbrt.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.fanxiaobao.xyz/Article/details/gowljzily.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezuknuni.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdeadzsd.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrvlvoft.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.fanxiaobao.xyz/Article/details/gszwaaxlt.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.fanxiaobao.xyz/Article/details/godwuvbdl.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfyocgoiu.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.fanxiaobao.xyz/Article/details/ggicinfjx.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.fanxiaobao.xyz/Article/details/gcuuttxca.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.fanxiaobao.xyz/Article/details/gbyaspmki.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.fanxiaobao.xyz/Article/details/ggbzaezih.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gcpbbtdkc.sHtML

K. JSON 与序列化
来源：http://read.share.fanxiaobao.xyz/Article/details/gpiwmdfls.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/grjuxrjce.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gqcequssz.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxemmsix.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.fanxiaobao.xyz/Article/details/gndaptnna.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gewgxlngk.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/geoqdjcfw.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqjrjkpg.sHtML

Go:   json.Marshal(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/grukiynon.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.fanxiaobao.xyz/Article/details/gngaoikko.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galosejty.sHtML


<!-- 参考信息 -->